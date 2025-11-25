

# Hoodl X MCP Integration

## Overview
Hoodl's Model Context Protocol (MCP) provides instant access to our comprehensive database of X (formerly Twitter) influencers. This tool allows you to query, filter, and export verified, active influencers from various niches including Web3, marketing, entertainment, and more.

## Features
- Access to thousands of verified influencers (5k+ followers, active last 30 days)
- Natural language queries to find exactly what you need
- Export functionality to CSV for immediate outreach
- Real-time data from our constantly updated database
- Unlimited queries with 1/sec rate limit

## Setup Instructions

### Prerequisites
- A valid Hoodl bearer token (30-day access for $39.99)
- An AI client that supports MCP integration (Claude, Qwen Code, Gemini CLI, etc.)

### Configuration
1. Purchase your token from [hoodl.net](https://hoodl.net)
2. Update your client's settings.json with the following configuration:

```json
{
  "mcpServers": {
    "x-influencer-mcp": {
      "httpUrl": "https://hoodl.net/mcp",
      "headers": {
        "authorization": "Bearer YOUR_API_KEY_HERE"
      }
    }
  },
  "privacy": {
    "usageStatisticsEnabled": false
  }
}
```

3. Replace `YOUR_API_KEY_HERE` with your actual Hoodl bearer token
4. Restart your AI client to establish the connection

## Response Format
The MCP will return structured data that can include:
- Influencer profiles with follower counts
- Engagement metrics
- Recent activity
- Contact information where available
- CSV export options

## Rate Limits
- Unlimited queries with a 1/sec rate limit
- Token valid for 30 days from activation

## Support
For technical issues or feature requests, please:
1. Submit an issue on our [GitHub repository](https://github.com/hoodl-dev/hoodl-x-mcp/issues)
2. Join our [Discord community](https://discord.gg/2R6QsHwa)

## About Hoodl
Hoodl is a powerful influencer discovery platform that uses advanced algorithms to identify, vet, and rank creators across X. Our database is constantly updated with verified, active accounts to ensure you get the most reliable data for your campaigns.

For more information about our other services, visit [hoodl.net](https://hoodl.net).
