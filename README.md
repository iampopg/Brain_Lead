# Brain Lead - All-in-One Email & SMS Tools 

![Brain Lead Logo](logo.png)

Brain Lead is a comprehensive windows application for lead generation, validation, and management. It provides powerful tools for generating, validating, and processing email addresses and phone numbers with advanced carrier detection and API integration capabilities.

## 🚀 Features

### Core Modules

- **📊 Dashboard**: Real-time statistics, activity monitoring, and tool usage tracking
- **🔄 Workflow**: Automated lead processing pipeline with validation and carrier filtering
- **📧 Email Generator**: Generate realistic or random email addresses with customizable domains
- **📱 Phone Generator**: Generate phone numbers with area codes and custom formatting
- **✅ Validator**: Multi-provider email/phone validation (Amazon, Microsoft)
- **📡 Carrier Checker**: Real-time carrier detection
- **🔍 Google Extractor**: Extract emails/phones from Google search results
- **🧹 Data Cleansing**: Clean, deduplicate, and format lead data
- **📮 Debounce Integration**: Email deliverability verification

### Advanced Features

- **🌐 Multi-language Support**: English, 中文 (Chinese), Français (French)
- **🔒 Security**: SSL verification, input validation, path sanitization
- **🎯 Proxy Support**: Rotate through proxy lists for validation
- **⚡ Multi-threading**: Concurrent processing for better performance
- **📈 Statistics Tracking**: Comprehensive usage analytics
- **🔄 Uniqueness Control**: Prevent duplicate lead generation
- **💾 Export Options**: Save results in various formats

## 📋 Requirements

### System Requirements

- **OS**: Windows 10/11
- **RAM**: 4GB minimum, 8GB recommended
- **Storage**: 500MB free space

## 🛠️ Installation

1. Download the latest release from GitHub
2. Extract the archive
3. Run `Brain_Lead.exe`

## ⚙️ Configuration

### Initial Setup

1. **Launch the application**
2. **Configure API credentials** in Settings:
   - Google API Key (for search extraction)
   - Google Search Engine ID
   - Debounce API Key (for email verification)

### Configuration Files

- `config/settings.json` - Main application settings
- `config/credentials_template.json` - Credential template
- `config/proxies.txt` - Proxy list for validation

### Environment Variables (Recommended for Production)

```cmd
set GOOGLE_API_KEY=your_google_api_key
set GOOGLE_ENGINE_ID=your_search_engine_id
set DEBOUNCE_API_KEY=your_debounce_api_key
```

## 🎯 Usage Guide

### Quick Start Workflow

1. **Generate Leads**: Use the Generator to create email/phone lists
2. **Validate**: Run validation to verify lead quality
3. **Check Carriers**: Identify phone carriers for SMS targeting
4. **Export Results**: Save validated leads for campaigns

### Module-Specific Usage

#### 📧 Email Generator

- **Realistic Mode**: Generates names like `john.smith@gmail.com`
- **Random Mode**: Creates random usernames
- **Custom Domains**: Specify target domains
- **Bulk Generation**: Generate thousands of emails

#### 📱 Phone Generator

- **Area Code Targeting**: Focus on specific regions
- **Custom Length**: Control number format
- **International Support**: Generate with country codes
- **Carrier Filtering**: Target specific carriers

#### ✅ Validation Engine

- **Multi-Provider**: Amazon, Microsoft validation
- **Validation Modes**:
  - Amazon Only
  - Microsoft Only
  - Amazon First (fallback to Microsoft)
  - Microsoft First (fallback to Amazon)
  - Both Required (strict validation)

#### 📡 Carrier Detection

- **Real-time Lookup**: Live carrier identification
- **Carrier Grouping**: Automatic carrier normalization
- **SMS Gateway**: Email-to-SMS conversion
- **Batch Processing**: Handle large datasets efficiently

#### 🔍 Google Extractor

- **Search Automation**: Extract from Google results
- **Auto-Dorks**: Intelligent search query generation
- **Domain Filtering**: Target specific websites
- **Data Extraction**: Emails, phones, and contact info

### 🔄 Automated Workflow

The Workflow module combines all tools into a single pipeline:

1. **Input Selection**: Generate or load existing leads
2. **Validation**: Multi-provider verification
3. **Carrier Filtering**: Target specific carriers
4. **Debounce Check**: Email deliverability verification
5. **Export**: Save final results



## 🔒 Security Features

### Input Validation

- **Email Format**: RFC-compliant regex validation
- **Phone Numbers**: Length and format validation
- **File Paths**: Sanitization and traversal protection
- **API Inputs**: Parameter validation and sanitization

### Network Security

- **SSL/TLS**: Certificate verification enabled
- **Request Timeouts**: Prevent hanging connections
- **Retry Logic**: Exponential backoff for failed requests
- **Secure Headers**: User-Agent and connection management

### Data Protection

- **Credential Management**: Secure storage in config files
- **Environment Variables**: Production credential handling
- **Path Validation**: Prevent directory traversal attacks
- **Error Handling**: Secure error messages

## 🌐 API Integrations

### Google Custom Search API

- **Search Automation**: Programmatic Google searches
- **Result Extraction**: Parse search results for contact data
- **Rate Limiting**: Respect API quotas and delays
- **Custom Engines**: Target specific websites

### Debounce Email Validation API

- **Deliverability Check**: Real-time email verification
- **Bounce Prediction**: Identify problematic addresses
- **Bulk Processing**: Handle large email lists
- **Detailed Results**: Comprehensive validation reports

### Carrier Database

- **Real-time Lookup**: Live carrier identification
- **Comprehensive Coverage**: US and international numbers
- **Batch Processing**: Efficient bulk lookups

## 📊 Statistics & Analytics

### Dashboard Metrics

- **Generation Stats**: Total leads generated
- **Validation Counts**: Valid/invalid ratios
- **Carrier Distribution**: Breakdown by carrier
- **Tool Usage**: Module activity tracking

### Export Formats

- **Text Files**: Simple line-separated lists
- **CSV**: Structured data with headers
- **JSON**: Programmatic data exchange
- **Carrier-Specific**: Organized by carrier

## 🚨 Troubleshooting

### Common Issues

#### SSL Certificate Errors

- Update Windows certificates through Windows Update
- Check system date and time settings

#### API Authentication Errors

- Verify API keys are correctly set
- Check API quotas and limits
- Ensure environment variables are loaded

#### Performance Issues

- Reduce thread count for slower systems
- Use proxy rotation to avoid rate limits
- Enable uniqueness checking to prevent duplicates

#### File Permission Errors

- Ensure write permissions for output directories
- Check file paths for special characters
- Use absolute paths when possible

### Debug Mode

Enable debug logging by setting environment variable:

```cmd
set BRAIN_DEBUG=1
```

## 🤝 Contributing

### Development Setup

1. Fork the repository
2. Create a feature branch
3. Install development dependencies
4. Make your changes
5. Run tests and security checks
6. Submit a pull request



## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🆘 Support

### Documentation

- **API Documentation**: Available in module docstrings
- **Configuration Guide**: See `config/` directory

### Contact

- **Telegram**: [@iampopg](https://t.me/iampopg)
- **Issues**: GitHub Issues page
- **Email**: Contact through Telegram for support

### Version History

- **v1.0**: Initial release with core functionality
- **Security Updates**: Enhanced input validation and SSL handling
- **Performance**: Multi-threading and batch processing improvements

## ⚠️ Disclaimer

This tool is for legitimate lead generation and validation purposes only. Users are responsible for:

- Complying with applicable laws and regulations
- Respecting website terms of service
- Following email marketing best practices
- Obtaining proper consent for communications

Use responsibly and ethically.

---

**Brain Lead** - Intelligent Lead Generation & Validation Platform
