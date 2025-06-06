# Cronhost Documentation

This repository contains the official documentation for [Cronhost](https://cronho.st) - a powerful service for scheduling HTTP requests using cron expressions.

## 📖 What's Included

- **Complete API Reference** - Interactive OpenAPI documentation with live examples
- **TypeScript SDK Guide** - Comprehensive SDK documentation with type definitions
- **Quickstart Guide** - Get up and running in under 5 minutes
- **Real-world Examples** - Practical use cases and code samples

## 🚀 Features Documented

- **Schedule Management** - Create, update, delete, and control HTTP request schedules
- **Cron Expressions** - Standard 5-field cron syntax with timezone support
- **Job Monitoring** - Track execution history, success rates, and error details
- **Error Handling** - Retry logic, timeouts, and comprehensive error responses
- **Authentication** - API key-based authentication with security best practices

## 🛠 Development

### Prerequisites

Install the [Mintlify CLI](https://www.npmjs.com/package/mintlify) to preview documentation changes locally:

```bash
npm i -g mintlify
```

### Local Development

Run the following command at the root of the documentation directory:

```bash
mintlify dev
```

This will start a local development server at `http://localhost:3000` where you can preview your changes in real-time.

### Project Structure

```
cronhost-docs/
├── index.mdx                    # Main landing page
├── quickstart.mdx              # Getting started guide
├── development.mdx             # Development best practices
├── docs.json                   # Documentation configuration
├── api-reference/              # REST API documentation
│   ├── introduction.mdx        # API overview
│   ├── authentication.mdx     # API key setup
│   ├── openapi.json           # OpenAPI specification
│   ├── schedule/              # Schedule endpoints
│   └── job/                   # Job endpoints
└── sdk-reference/             # TypeScript SDK documentation
    ├── introduction.mdx       # SDK setup
    ├── schedules.mdx         # Schedule management
    ├── jobs.mdx              # Job monitoring
    └── types.mdx             # Type definitions
```

## 📝 Documentation Guidelines

### Writing Style
- Use clear, concise language
- Include practical code examples
- Provide both cURL and SDK examples where applicable
- Focus on real-world use cases

### Code Examples
- Always include working code examples
- Use TypeScript for SDK examples
- Include error handling patterns
- Show both success and error scenarios

### OpenAPI Specification
- Keep `openapi.json` up to date with the latest API changes
- Include comprehensive examples for all endpoints
- Document all request/response schemas
- Provide multiple example scenarios

## 🚢 Publishing Changes

### Automatic Deployment
Changes are automatically deployed to production when pushed to the main branch. The Mintlify GitHub App handles the deployment process.

### Manual Deployment
If needed, you can manually trigger a deployment from the [Mintlify dashboard](https://dashboard.mintlify.com).

## 📚 Related Resources

- **Cronhost Website**: [cronho.st](https://cronho.st)
- **Dashboard**: [cronho.st/dashboard](https://cronho.st/dashboard)
- **API Base URL**: `https://cronho.st/api/v1`
- **Support**: [help@cronho.st](mailto:help@cronho.st)
- **Status Page**: [status.cronho.st](https://status.cronho.st)

## 🔧 Troubleshooting

### Common Issues

**Mintlify dev isn't running**
```bash
mintlify install
```
This will re-install dependencies.

**Page loads as 404**
- Ensure you're running the command in a folder with `docs.json`
- Check that all file paths in `docs.json` are correct
- Verify that referenced files exist

**OpenAPI endpoints not showing**
- Validate your `openapi.json` syntax
- Ensure endpoint files reference the correct OpenAPI operations
- Check that the OpenAPI spec is properly linked in `docs.json`

### Getting Help

- **Documentation Issues**: Open an issue in this repository
- **Mintlify Questions**: Check the [Mintlify documentation](https://mintlify.com/docs)
- **Cronhost API Issues**: Contact [help@cronho.st](mailto:help@cronho.st)

## 📄 License

This documentation is maintained by the Cronhost team. For licensing information about the Cronhost service, please refer to our [terms of service](https://cronho.st/terms).

---

Made with ❤️ by the Cronhost team