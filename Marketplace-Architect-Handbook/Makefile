BOOK_FILES = INTRODUCTION.md \
	00-Founder-Mindset.md 01-Market-Research.md 02-Category-Architecture.md \
	03-Business-Model.md 04-Unit-Economics.md 05-Demand-Generation.md \
	06-Supply-Acquisition.md 07-Worker-Vetting.md 08-Trust-Safety.md \
	09-Fraud.md 10-Legal.md 11-Contracts.md 12-Matching-Engine.md \
	13-Pricing.md 14-Payments.md 15-Warranty.md 16-Insurance.md \
	17-Disputes.md 18-Product.md 19-UX.md 20-Operations.md \
	21-City-Launch.md 22-Scaling.md 23-Analytics.md \
	24-Worker-Retention.md 25-Customer-Retention.md 26-B2B.md \
	27-Cybersecurity.md 28-AI.md 29-Financial-Modeling.md \
	30-Fundraising.md 31-Failure-Case-Studies.md 32-Exit-Strategy.md \
	Glossary/Glossary.md Appendix/Acronyms-Abbreviations.md Appendix/Master-Index.md \
	References/References.md Bibliography/Bibliography.md

OUTPUT_DIR = dist
TITLE = The-Marketplace-Architect-Handbook

.PHONY: all pdf docx a4 clean

all: pdf docx a4

$(OUTPUT_DIR):
	mkdir -p $(OUTPUT_DIR)

pdf: $(OUTPUT_DIR)
	pandoc $(BOOK_FILES) --toc --number-sections -V geometry:a4paper -V geometry:margin=1in -o $(OUTPUT_DIR)/$(TITLE).pdf

docx: $(OUTPUT_DIR)
	pandoc $(BOOK_FILES) --toc --number-sections -o $(OUTPUT_DIR)/$(TITLE).docx

a4: $(OUTPUT_DIR)
	pandoc $(BOOK_FILES) --toc --number-sections -V papersize:a4 -V geometry:margin=0.75in -o $(OUTPUT_DIR)/$(TITLE)-A4.pdf

clean:
	rm -rf $(OUTPUT_DIR)
