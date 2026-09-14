# PageSpeed Insights MCP Server by Insightful Pipe

[![MCP Compatible](https://img.shields.io/badge/MCP-Compatible-blue)](https://insightfulpipe.com/mcp-servers/pagespeed)
[![Insightful Pipe](https://img.shields.io/badge/Insightful_Pipe-MCP_Servers-purple)](https://insightfulpipe.com/mcp-servers)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

> **Analyze website performance and Core Web Vitals with AI through MCP.**

Part of the [Insightful Pipe MCP Server Collection](https://insightfulpipe.com/mcp-servers) — The PageSpeed Insights MCP server enables Claude, ChatGPT, Cursor, and other AI assistants to analyze website performance. Get Core Web Vitals, performance scores, and AI-powered optimization recommendations.

[![Explore All MCP Servers](https://img.shields.io/badge/Explore_All-MCP_Servers-blue?style=for-the-badge)](https://insightfulpipe.com/mcp-servers)

![PageSpeed Insights MCP Server](https://insightfulpipe.com/images/google-pagespeed-insights-icon-2021-.svg)

## MCP Server URL

```
https://pagespeed-insights.insightfulmcp.com/
```

## What is PageSpeed Insights MCP?

PageSpeed Insights MCP is a **remote Model Context Protocol server** that provides AI assistants with website performance analysis capabilities. This performance optimization integration allows you to:

- Analyze page speed and Core Web Vitals
- Get detailed Lighthouse performance breakdowns
- Receive AI-powered optimization recommendations
- Check accessibility and SEO scores
- Identify resource optimization opportunities

## Installation

### Claude

1. Copy the MCP Server URL: `https://pagespeed-insights.insightfulmcp.com/`
2. Open [Claude Connectors Settings](https://claude.ai/settings/connectors)
3. Scroll to the bottom and click **Add custom connector**
4. Paste the URL and click **Add**
5. Click **Connect** on the connector to start authorization
6. Click **Authorize access** in the browser to complete the connection

### ChatGPT

Custom MCP servers are added through ChatGPT's **Developer mode**. Availability depends on your ChatGPT plan, and workspace admins may need to allow it.

1. Turn on **Developer mode** in ChatGPT settings
2. Create a new app for a remote MCP server and paste the URL: `https://pagespeed-insights.insightfulmcp.com/`
3. Authorize with your InsightfulPipe account

See OpenAI's guide: [Developer mode and MCP apps in ChatGPT](https://help.openai.com/en/articles/12584461-developer-mode-and-mcp-apps-in-chatgpt)

### Claude Code

```bash
claude mcp add --transport http pagespeed https://pagespeed-insights.insightfulmcp.com/
```

### Cursor

Add the server to `~/.cursor/mcp.json` (all projects) or `.cursor/mcp.json` (one project):

```json
{
  "mcpServers": {
    "pagespeed": {
      "url": "https://pagespeed-insights.insightfulmcp.com/"
    }
  }
}
```

Then authorize the connection when Cursor prompts you.

## Available Actions

4 actions: 4 read, 0 write.

### Read Actions (4)

| Action | Description |
|--------|-------------|
| `accessibility-seo` | Accessibility and SEO category scores with failing audits |
| `analyze.full` | Full Lighthouse payload across all categories |
| `core-web-vitals` | Core Web Vitals snapshot (FCP, LCP, CLS, TTI, TBT, Speed Index, TTFB) |
| `resource-optimizations` | Resource-focused audits (render-blocking, unused JS/CSS, caching, images) |

## Control What Your AI Can Do

You decide what AI agents can do with each connected account:

- **Turn individual actions on or off** for every connected account, so agents only see the actions you allow.
- **Connect as Read-only or Read & Write.** A read-only connection can only enable read actions.
- **Destructive actions stay off by default.** Actions such as deletes are disabled until an admin enables them.
- **Team access per account.** Restricted team members only use the accounts they are granted, with the read actions enabled on them.

## Usage Examples

### Performance Analysis

```
"Analyze the page speed of https://example.com"
```

### Core Web Vitals Check

```
"What are the Core Web Vitals for my homepage?"
```

### Resource Optimization

```
"What resources are slowing down my page?"
```

### Full Lighthouse Audit

```
"Run a full Lighthouse audit on this URL"
```

### Accessibility Check

```
"Check the accessibility score for this page"
```

## Core Web Vitals

| Metric | Description | Good Threshold |
|--------|-------------|----------------|
| LCP | Largest Contentful Paint | < 2.5s |
| FID/INP | First Input Delay / Interaction to Next Paint | < 100ms |
| CLS | Cumulative Layout Shift | < 0.1 |
| TTFB | Time to First Byte | < 800ms |
| FCP | First Contentful Paint | < 1.8s |
| TTI | Time to Interactive | < 3.8s |
| TBT | Total Blocking Time | < 200ms |
| Speed Index | Visual loading speed | < 3.4s |

## Why PageSpeed Insights MCP?

### For Web Developers
- **Performance monitoring** - Track site speed
- **Debug slow pages** - Identify bottlenecks
- **Optimization guidance** - Know what to fix

### For SEO Professionals
- **Core Web Vitals** - Critical ranking factor
- **Mobile performance** - Mobile-first indexing
- **Technical SEO** - Performance auditing

### For Marketers
- **Conversion optimization** - Speed impacts conversions
- **User experience** - Better page experience
- **Competitive analysis** - Compare against competitors

## Security & Privacy

- **Google API** - Official PageSpeed Insights API
- **Public page analysis** - Only public URLs

## Ready-Made Skills and Prompts

- [Claude skills for SEO and marketing](https://insightfulpipe.com/marketing-claude-skills/marketing) — ready-made skills that run on your connected data
- [Core Web Vitals Assessment](https://insightfulpipe.com/marketing-prompts-library/pagespeed-core-web-vitals-assessment)
- [Full Lighthouse Performance Audit](https://insightfulpipe.com/marketing-prompts-library/pagespeed-full-lighthouse-performance-audit)
- [Mobile Vs Desktop Performance Comparison](https://insightfulpipe.com/marketing-prompts-library/pagespeed-mobile-vs-desktop-performance-comparison)

## Explore More MCP Servers by Insightful Pipe

Visit **[insightfulpipe.com/mcp-servers](https://insightfulpipe.com/mcp-servers)** to discover our full collection of MCP servers for marketing and analytics.

### SEO & Performance MCP Servers
- [Google Search Console MCP](https://insightfulpipe.com/mcp-servers/google-search-console) - SEO analytics
- [Web Crawler MCP](https://insightfulpipe.com/mcp-servers/crawler) - Site crawling
- [Screenshot MCP](https://insightfulpipe.com/mcp-servers/screenshot) - Visual capture

### Analytics MCP Servers
- [Google Analytics MCP](https://insightfulpipe.com/mcp-servers/google-analytics) - Website analytics
- [Google My Business MCP](https://insightfulpipe.com/mcp-servers/google-my-business) - Local SEO

**[View All MCP Servers →](https://insightfulpipe.com/mcp-servers)**

## Resources

- [Documentation](https://insightfulpipe.com/docs/connectors-pagespeed-insights)
- [Video Tutorial](https://www.youtube.com/playlist?list=PLJNzvjxzI5Xwe__BJJLAelSF0ewO3mEFk)
- [InsightfulPipe Blog](https://insightfulpipe.com/blog)

## Support

- **Documentation**: [insightfulpipe.com/docs](https://insightfulpipe.com/docs)
- **All MCP Servers**: [insightfulpipe.com/mcp-servers](https://insightfulpipe.com/mcp-servers)
- **Email**: support@insightfulpipe.com

---

**[Insightful Pipe](https://insightfulpipe.com)** — AI-powered marketing analytics through MCP servers. [Explore all integrations →](https://insightfulpipe.com/mcp-servers)

## License

MIT License - see [LICENSE](LICENSE) for details.
