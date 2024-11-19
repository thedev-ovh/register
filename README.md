# thedev.ovh - Free Subdomain Service

Welcome to **thedev.ovh**! We provide free subdomains with easy-to-use DNS management. You can create subdomains with a variety of DNS records and configure your domain exactly the way you want.

### Features
- Free subdomains under `thedev.ovh`
- Support for a variety of DNS record types: **A**, **AAAA**, **CNAME**, **MX**, **TXT**
- Easy management through JSON configuration
- Proxied (Cloudflare) support for added security and speed

## How to Use

### Step 1: Fork the Repository
1. Visit our [GitHub repository](https://github.com/thedev-ovh)
2. Click the **Fork** button in the top right to make your own copy of the repository.

### Step 2: Create Your Subdomain Configuration
1. In your forked repository, navigate to the `subdomains` directory (or create it if it doesn't exist).
2. Create a new file with a `.json` extension for your subdomain. Example: `subdomain.thedev.ovh.json`.
3. Use the following template to add your subdomain and DNS records:

```json
{
  "subdomain": "yoursubdomain",
  "domain": "thedev.ovh",
  "email_or_discord": "user@example.com or user",
  "github_username": "user",
  "description": "A brief description of the purpose of the subdomain",

  "records": {
    "A":     ["1.0.0.1", "1.0.0.2"],
    "AAAA":  ["2000:db8::1", "2000:db8::2"],
    "CNAME": ["example.com"],
    "MX": ["mail1.example.com", "mail2.example.com"],
    "TXT":   ["v=spf1 include:_spf.example.com ~all"]
  },

  "proxied": true
}

**Note:** Please remove the "," at the end of the `.json` file when ending the record.

`"A":     ["1.0.0.1", "1.0.0.2"]`

### Contact us
If you have any problem to contact us, please contact us by email: admin@thedev.ovh - you will receive support soon.
