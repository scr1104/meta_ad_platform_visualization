# Meta Ad Platform Visualization

Interactive LEGO timeline visualization for daily ad spend analysis.

## Usage
- Upload your CSV with daily spend data
- Explore different CAC metrics and spend patterns
- Use interactive controls for filtering and sorting

## Live Demo
[View Timeline](https://scr1104.github.io/meta_ad_platform_visualization/index.html)

## Data Format
Expected CSV columns: ad_id, ad_name, ad_set_name, date_day, daily_spend, lifetime_cac_*

# Data Privacy & Security

This document outlines the comprehensive privacy and security measures built into the Ad Creative Daily Timeline visualization tool.

## Zero Data Collection Policy

**Your data never leaves your device.** This visualization tool is designed with privacy-first principles:

- **No server-side processing** - All data analysis happens locally in your browser
- **No data transmission** - Your CSV files are processed entirely on your device
- **No external storage** - No databases, cloud storage, or third-party services store your data
- **No tracking or analytics** - Zero cookies, session storage, or user behavior tracking
- **No user accounts** - No registration, login, or personal information collection

## How Data Processing Works

1. **File Upload**: When you drop or select a CSV file, it's read directly by your browser's JavaScript engine
2. **Local Processing**: All data parsing, calculations, and visualizations happen in your browser's memory
3. **Temporary Storage**: Data exists only in browser RAM while the page is active
4. **Automatic Cleanup**: All data is immediately destroyed when you:
   - Close the browser tab
   - Navigate away from the page
   - Refresh the page
   - Close your browser

## Technical Security Measures

### Client-Side Only Architecture
```
Your Device: CSV File → Browser Memory → Visualization Display
No Network: ❌ No data sent to servers
No Storage: ❌ No data saved anywhere
```

### External Dependencies
The tool loads only one external resource:
- **D3.js visualization library** from public CDN
- This is a standard, open-source charting library with no tracking capabilities
- No user data is sent to the CDN - only the library code is downloaded

### Browser Security
- Runs within browser's security sandbox
- Cannot access other tabs, applications, or system files
- Cannot make unauthorized network requests
- Cannot install software or modify your system

## Data Handling Guarantees

### What We DON'T Collect
- Ad spend amounts or financial data
- Campaign performance metrics
- Ad creative names or identifiers
- Customer acquisition costs (CAC)
- Click and conversion data
- Company or advertiser names
- Any personally identifiable information

### What We DON'T Store
- No server logs of file uploads
- No cached visualization data
- No user sessions or preferences
- No IP addresses or device information
- No usage analytics or metrics

### What We DON'T Share
Since no data is collected or stored, there is nothing to share with:
- Third-party services
- Analytics providers
- Advertising networks
- Data brokers
- Government agencies (unless legally required for the static hosting service)

## Hosting & Infrastructure

### GitHub Pages Hosting
- **Static file hosting only** - No server-side processing capabilities
- **No database** - GitHub Pages cannot store user data
- **No server logs** - Standard web server logs may include page visits but not file contents
- **HTTPS encryption** - All data transmission between your browser and GitHub is encrypted

### Open Source Transparency
- Complete source code is publicly available
- No hidden functionality or obfuscated code
- Community-auditable for security concerns
- No proprietary tracking or data collection libraries

## Compliance & Standards

### Privacy Regulations
This tool complies with major privacy regulations by design:
- **GDPR** - No personal data processing or storage
- **CCPA** - No sale or sharing of personal information
- **PIPEDA** - No collection of personal information
- **SOX/HIPAA** - Can be used with sensitive financial/health data as it remains on-device

### Industry Standards
- Follows OWASP security guidelines for web applications
- Implements Content Security Policy (CSP) best practices
- Uses secure HTTPS connections only
- No use of deprecated or insecure web technologies

## Risk Assessment

### Minimal Risk Profile
- **Data Breach Risk**: Zero - no centralized data storage
- **Unauthorized Access**: Impossible - data never transmitted
- **Data Corruption**: Limited to user's local session only
- **Privacy Violation**: None - no data collection mechanism exists

### Theoretical Risks
1. **Browser Vulnerabilities**: Like any web application, relies on browser security
2. **Network Interception**: Mitigated by HTTPS encryption for page loading
3. **Local Device Security**: Your device's existing security applies

## Recommendations for Users

### Best Practices
1. **Use updated browsers** with current security patches
2. **Verify HTTPS connection** (look for lock icon in browser)
3. **Close browser tab** when finished to clear memory
4. **Use on trusted networks** when accessing the tool

### For Sensitive Data
- The tool is designed to be safe for confidential business data
- No additional precautions needed beyond normal device security
- Can be used offline after initial page load (D3.js caches locally)

## Verification

### How to Verify Privacy Claims
1. **Network Monitoring**: Use browser developer tools (F12) to monitor network activity
2. **Source Code Review**: Examine the complete code on GitHub
3. **Browser Storage**: Check that no data persists in cookies/localStorage
4. **Memory Usage**: Observe memory cleanup when closing the tab

### Contact for Security Concerns
If you discover any security vulnerabilities or have privacy concerns:
- Review the source code on GitHub
- Open an issue in the repository
- Verify claims through independent technical analysis

## Summary

This visualization tool prioritizes data privacy through technical design rather than policy promises. By processing everything locally and collecting nothing remotely, it eliminates most privacy risks inherent in web-based tools. Your sensitive advertising and performance data remains under your complete control at all times.
