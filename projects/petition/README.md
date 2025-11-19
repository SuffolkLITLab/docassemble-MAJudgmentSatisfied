# docassemble.PetitionToDeemSatisfied

**Version:** 1.3.1  
**Author:** LIT Lab  
**License:** MIT

## Overview

This Docassemble interview helps tenants who have already paid an eviction judgment request that the court officially mark the judgment as satisfied. Once marked satisfied, it's easier to show future landlords or credit screeners that the case was resolved.

## What This Form Does

The **Petition to Deem Judgment Satisfied** is a Massachusetts Housing Court form that allows tenants to request the court mark their eviction judgment as satisfied after full payment. This is authorized under Massachusetts General Law [Chapter 239, Section 16(k)](https://malegislature.gov/Laws/GeneralLaws/PartIII/TitleIII/Chapter239/Section16).

## Who Can Use This

You are in the right place if:
- The case was for nonpayment of rent
- A judgment entered against you
- You paid the full judgment amount (including any agreed interest or costs)

## What You'll Need

Before starting, gather:
- Your court papers with the docket number
- Proof of payment (receipt, money order stub, bank record)
- The mailing or email address for the plaintiff or their attorney

## How It Works

The interview guides you through:

1. **Court and case information** - Court name, docket number, and parties
2. **Payment information** - Date you paid the judgment
3. **Your contact information** - Address, phone, and email
4. **Attorney information** (optional) - If you have an attorney
5. **Service information** - How you'll notify the other party (required before filing)
6. **Review and sign** - Double-check your answers and sign electronically
7. **Download** - Get your completed petition ready to serve and file

**Time estimate:** 10-15 minutes

## Installation

### For Docassemble Playground

1. Download the latest release zip file (`petition_to_deem_satisfied_v1.3.1.zip`)
2. Upload it to your Docassemble playground
3. The interview will be available immediately

### For Local Development

```bash
pip install -e .
```

## Dependencies

- `docassemble.AssemblyLine>=3.2.0`

## Features

- ✅ Left navigation sidebar for easy section tracking
- ✅ Bootstrap 3 panels for clear information display
- ✅ Enhanced alert cards for important tips and reminders
- ✅ Conditional logic for optional attorney information
- ✅ Multiple service methods (mail, email, in person)
- ✅ Electronic signature support
- ✅ PDF generation with properly labeled form fields

## Technical Details

### PDF Template

The interview uses `Petition-To-Deem-Satisfied-v1.3.pdf` with 25 properly labeled form fields:
- Court information (docket number, department, division)
- Party information (plaintiff, defendant/petitioner)
- Payment date
- Petitioner contact information
- Optional attorney information
- Certificate of service details

### Field Mapping

All PDF fields use semantic, professional naming conventions:
- No typos (e.g., "defendant" not "defendent")
- Consistent terminology (e.g., "attorney" not "lawyer")
- Clear prefixes (e.g., "service_*" for service-related fields)

## Version History

- **1.3.1** - Fixed undefined `service_address` variable in review screen
- **1.3** - Renamed all PDF fields to semantic names, fixed typos, standardized terminology
- **1.2.1** - Enhanced intro screen with Bootstrap panels and alert cards
- **1.2** - Added left navigation, removed numbered steps
- **1.1** - Initial release

## Support

For issues or questions, contact the LIT Lab at litlab@suffolklitlab.org

## License

MIT License - See LICENSE file for details
