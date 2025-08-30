# Healthcare AI Agents Security Verification Standard (HAAISVS) Makefile
# Build and validation tools for HAAISVS documentation and compliance verification

# Variables
HAAISVS_VERSION = 1.0
LANG = en
BUILD_DIR = build
SRC_DIR = $(HAAISVS_VERSION)/$(LANG)
TOOLS_DIR = $(HAAISVS_VERSION)/tools

# Default target
.PHONY: all
all: validate build

# Validation targets
.PHONY: validate
validate: validate-structure validate-requirements validate-mappings

.PHONY: validate-structure
validate-structure:
	@echo "Validating HAAISVS directory structure..."
	@test -d $(SRC_DIR) || (echo "Error: Source directory $(SRC_DIR) not found" && exit 1)
	@test -f $(SRC_DIR)/0x00-Header.yaml || (echo "Error: Header file missing" && exit 1)
	@test -f $(SRC_DIR)/0x01-Frontispiece.md || (echo "Error: Frontispiece missing" && exit 1)
	@test -f $(SRC_DIR)/0x03-Using-HAAISVS.md || (echo "Error: Usage guide missing" && exit 1)
	@test -f $(SRC_DIR)/0x10-C01-Risk-Lifecycle-Assessment.md || (echo "Error: C1 category missing" && exit 1)
	@test -f $(SRC_DIR)/0x10-C02-Model-Passport-Traceability.md || (echo "Error: C2 category missing" && exit 1)
	@test -f $(SRC_DIR)/0x10-C03-Cybersecurity-Framework.md || (echo "Error: C3 category missing" && exit 1)
	@test -f $(SRC_DIR)/0x10-C04-Human-Oversight.md || (echo "Error: C4 category missing" && exit 1)
	@echo "✓ Structure validation passed"

.PHONY: validate-requirements
validate-requirements:
	@echo "Validating verification requirements format..."
	@python3 $(TOOLS_DIR)/validate_requirements.py $(SRC_DIR)
	@echo "✓ Requirements validation passed"

.PHONY: validate-mappings  
validate-mappings:
	@echo "Validating regulatory framework mappings..."
	@python3 $(TOOLS_DIR)/validate_mappings.py $(HAAISVS_VERSION)/mappings
	@echo "✓ Mappings validation passed"

# Build targets
.PHONY: build
build: build-pdf build-html build-compliance-tools

.PHONY: build-pdf
build-pdf:
	@echo "Building HAAISVS PDF documentation..."
	@mkdir -p $(BUILD_DIR)
	@pandoc --template=$(HAAISVS_VERSION)/templates/haaisvs.tex \
		--from markdown --to latex \
		--output $(BUILD_DIR)/HAAISVS-$(HAAISVS_VERSION)-$(LANG).pdf \
		$(SRC_DIR)/*.md
	@echo "✓ PDF build completed: $(BUILD_DIR)/HAAISVS-$(HAAISVS_VERSION)-$(LANG).pdf"

.PHONY: build-html
build-html:
	@echo "Building HAAISVS HTML documentation..."
	@mkdir -p $(BUILD_DIR)/html
	@python3 $(TOOLS_DIR)/build_html.py $(SRC_DIR) $(BUILD_DIR)/html
	@echo "✓ HTML build completed: $(BUILD_DIR)/html/"

.PHONY: build-compliance-tools
build-compliance-tools:
	@echo "Building HAAISVS compliance verification tools..."
	@python3 $(TOOLS_DIR)/build_compliance_tools.py
	@echo "✓ Compliance tools built"

# Testing targets
.PHONY: test
test: test-requirements test-mappings test-tools

.PHONY: test-requirements
test-requirements:
	@echo "Testing verification requirements coverage..."
	@python3 $(TOOLS_DIR)/test_requirements_coverage.py $(SRC_DIR)
	@echo "✓ Requirements testing passed"

.PHONY: test-mappings
test-mappings:
	@echo "Testing regulatory mappings accuracy..."
	@python3 $(TOOLS_DIR)/test_mappings_accuracy.py $(HAAISVS_VERSION)/mappings
	@echo "✓ Mappings testing passed"

.PHONY: test-tools
test-tools:
	@echo "Testing compliance verification tools..."
	@python3 $(TOOLS_DIR)/test_compliance_tools.py
	@echo "✓ Tools testing passed"

# Quality assurance targets
.PHONY: qa
qa: lint spell-check link-check

.PHONY: lint
lint:
	@echo "Linting HAAISVS markdown files..."
	@markdownlint $(SRC_DIR)/*.md
	@echo "✓ Markdown linting passed"

.PHONY: spell-check
spell-check:
	@echo "Spell checking HAAISVS documentation..."
	@aspell check $(SRC_DIR)/*.md
	@echo "✓ Spell check completed"

.PHONY: link-check
link-check:
	@echo "Checking internal and external links..."
	@python3 $(TOOLS_DIR)/check_links.py $(SRC_DIR)
	@echo "✓ Link checking passed"

# Release targets
.PHONY: release
release: validate test qa build package

.PHONY: package
package:
	@echo "Packaging HAAISVS $(HAAISVS_VERSION) release..."
	@mkdir -p $(BUILD_DIR)/release
	@tar -czf $(BUILD_DIR)/release/HAAISVS-$(HAAISVS_VERSION).tar.gz \
		$(HAAISVS_VERSION)/ \
		README.md \
		LICENSE.md
	@echo "✓ Release package created: $(BUILD_DIR)/release/HAAISVS-$(HAAISVS_VERSION).tar.gz"

# Development targets
.PHONY: serve
serve:
	@echo "Starting HAAISVS documentation server..."
	@python3 -m http.server 8080 --directory $(BUILD_DIR)/html
	@echo "Documentation available at http://localhost:8080"

.PHONY: watch
watch:
	@echo "Watching for changes and rebuilding..."
	@python3 $(TOOLS_DIR)/watch_and_build.py $(SRC_DIR) $(BUILD_DIR)

# Utility targets
.PHONY: clean
clean:
	@echo "Cleaning build artifacts..."
	@rm -rf $(BUILD_DIR)
	@echo "✓ Build directory cleaned"

.PHONY: stats
stats:
	@echo "HAAISVS $(HAAISVS_VERSION) Statistics:"
	@echo "Total verification requirements: $$(python3 $(TOOLS_DIR)/count_requirements.py $(SRC_DIR))"
	@echo "Regulatory mappings: $$(ls -1 $(HAAISVS_VERSION)/mappings/*.json | wc -l)"
	@echo "Documentation files: $$(ls -1 $(SRC_DIR)/*.md | wc -l)"

.PHONY: help
help:
	@echo "HAAISVS $(HAAISVS_VERSION) Build System"
	@echo ""
	@echo "Validation:"
	@echo "  validate              - Run all validation checks"
	@echo "  validate-structure    - Check directory structure"
	@echo "  validate-requirements - Check verification requirements format"
	@echo "  validate-mappings     - Check regulatory mappings"
	@echo ""
	@echo "Build:"
	@echo "  build                 - Build all documentation formats"
	@echo "  build-pdf             - Build PDF documentation"
	@echo "  build-html            - Build HTML documentation"
	@echo "  build-compliance-tools - Build compliance verification tools"
	@echo ""
	@echo "Testing:"
	@echo "  test                  - Run all tests"
	@echo "  test-requirements     - Test requirements coverage"
	@echo "  test-mappings         - Test mapping accuracy"
	@echo "  test-tools            - Test compliance tools"
	@echo ""
	@echo "Quality Assurance:"
	@echo "  qa                    - Run all QA checks"
	@echo "  lint                  - Lint markdown files"
	@echo "  spell-check           - Check spelling"
	@echo "  link-check            - Check links"
	@echo ""
	@echo "Release:"
	@echo "  release               - Full release build"
	@echo "  package               - Create release package"
	@echo ""
	@echo "Development:"
	@echo "  serve                 - Serve documentation locally"
	@echo "  watch                 - Watch and rebuild on changes"
	@echo ""
	@echo "Utility:"
	@echo "  clean                 - Clean build artifacts"
	@echo "  stats                 - Show HAAISVS statistics"
	@echo "  help                  - Show this help message"

# Default help target
.DEFAULT_GOAL := help
