# Web Modules CDN

A comprehensive CDN hosting three powerful web widgets for campaign management, market research, and creative brief generation.

## Modules

### 1. Campaign Intelligence Widget
A powerful widget for managing and analyzing campaign intelligence data.

**CDN Links:**
```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/shailesh12312/web-modules-cdn@main/campaign-intelligence/style.css">
<script src="https://cdn.jsdelivr.net/gh/shailesh12312/web-modules-cdn@main/campaign-intelligence/campaign-intelligence.umd.js"></script>
```

**Mount Point:**
```javascript
window.CampaignIntelligence.mount('campaign-intelligence-root', {
    subscription_id: 'your-subscription-id',
    token: 'your-token',
    market_intelligence_location: 'http://your-domain/market-intelligence',
    creative_brief_location: 'http://your-domain/creative-brief',
});
```

---

### 2. Creative Brief Widget
A comprehensive widget for creating and managing creative briefs.

**CDN Links:**
```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/shailesh12312/web-modules-cdn@main/creative-brief/style.css">
<script src="https://cdn.jsdelivr.net/gh/shailesh12312/web-modules-cdn@main/creative-brief/creative-brief.umd.js"></script>
```

**Mount Point:**
```javascript
window.CreativeBriefWidget.mount('creative-brief-root', {
    subscription_id: 'your-subscription-id',
    token: 'your-token',
    campaign_intelligence_location: 'http://your-domain/campaign-intelligence',
});
```

---

### 3. Market Intelligence Widget
An advanced widget for market research and intelligence gathering.

**CDN Links:**
```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/shailesh12312/web-modules-cdn@main/market-intelligence/style.css">
<script src="https://cdn.jsdelivr.net/gh/shailesh12312/web-modules-cdn@main/market-intelligence/market-intelligence.umd.js"></script>
```

**Mount Point:**
```javascript
window.MarketIntelligenceWidget.mount('market-intelligence-root', {
    subscription_id: 'your-subscription-id',
    token: 'your-token',
    campaign_intelligence_location: 'http://your-domain',
});
```

---

## Quick Start

### HTML Template
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Campaign Intelligence</title>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/shailesh12312/web-modules-cdn@main/campaign-intelligence/style.css">
</head>
<body>
    <div id="campaign-intelligence-root"></div>
    <script src="https://cdn.jsdelivr.net/gh/shailesh12312/web-modules-cdn@main/campaign-intelligence/campaign-intelligence.umd.js"></script>
    <script>
        if (window.CampaignIntelligence) {
            window.CampaignIntelligence.mount('campaign-intelligence-root', {
                subscription_id: 'your-subscription-id',
                token: 'your-token',
                market_intelligence_location: 'http://your-domain/market-intelligence',
                creative_brief_location: 'http://your-domain/creative-brief',
            });
        } else {
            console.error('CampaignIntelligence not found on window');
        }
    </script>
</body>
</html>
```

## Features

- **Campaign Intelligence**: Comprehensive campaign analytics and insights
- **Creative Brief**: Streamlined creative brief creation and management
- **Market Intelligence**: Market trend analysis and competitive intelligence
- **Responsive Design**: Works seamlessly on all modern browsers
- **Easy Integration**: Simple CDN-based integration with minimal setup

## Browser Support

All modules support modern browsers:
- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## Configuration

Each widget accepts the following configuration options:

| Option | Type | Description |
|--------|------|-------------|
| `subscription_id` | string | Your subscription ID for authentication |
| `token` | string | Your Token for authentication |
| `market_intelligence_location` | string | URL to the Market Intelligence module |
| `creative_brief_location` | string | URL to the Creative Brief module |
| `campaign_intelligence_location` | string | URL to the Campaign Intelligence module |

## License

All rights reserved.
