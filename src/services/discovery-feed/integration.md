# Discovery Feed Integration

Integrating our personalized Discovery Feed allows you to provide users with relevant news and offers, enhancing engagement on your platform.

## Filtering Posts

As the host of the discovery feed, you can manage which posts are displayed, including:

- **Blacklists**: Prevent certain projects or topics from appearing.
- **Whitelists**: Specify only particular projects or topics that you want to display.

## Integration

Integrating the Discovery Feed into your web page is similar to setting up an ad unit.

1. **Set up a New Ad Unit**: Follow the steps from the [ad unit guide](../ads/publisher.md).
2. **Add the Integration Snippet**: Insert you ad unit id into the snippet below and add it to your webpage:

    ```html
    <Feed
        unitId="YOUR UNIT ID HERE"
    />
    ```

For an example of integration, check out our [GitHub](https://github.com/growth-mate/react-example).