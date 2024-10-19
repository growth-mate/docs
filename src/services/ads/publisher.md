# Publish for GrowthMate

Becoming a publisher in our Ad-Network allows you to turn your traffic into revenue, or promote internal features. By leveraging AI, the network ensures that users see ads aligned with their interests, leading to increased engagement and higher returns for your platform.

## Publisher Controls

As a publisher, you have the ability to manage the types of ads displayed on your platform, including:

- **Blacklists**: Prevent certain projects or topics from appearing. (e.g. competitors)
- **Whitelists**: Specify only particular projects or topics that you want to display. (e.g. partners)

## Integration

```admonish note
We recommend using separate ad units for mobile and desktop pages. This lets you utilize different ad formats and receive distinct performance reports for better insights.
```

Integrating our ad units into your web page is simple. Follow these steps:

1. **Create a New Ad Unit**: Go to our [publisher dashboard](https://growthmate.xyz/publish) and create a new ad unit.
2. **Provide Backup Options**: Supply a backup link and image, which will be displayed if there are any issues during the recommendation process.
3. **Add the Integration Snippet**: Copy the snippet from the dashboard and paste it into your webpage. It should look something like this:

    ```html
    <Ad
        unitId="YOUR UNIT ID HERE"
        format="Leaderboard"
    />
    ```

For an example of integration, check out our [GitHub](https://github.com/growth-mate/react-example).


## Ad Unit Styling

You may apply custom styling to your ad unit. The easiest way is through the `.gm-ad-unit` CSS class. Additionally, you may use the data attributes `data-gm-is-backup` and `data-gm-is-error` to adjust the styling in case the ad unit shows your backup media or there was a fatal error. Example:

```css
.gm-ad-unit[data-gm-is-error="true"] {
    visibility: hidden;
}
```

```admonish warning title="Restrictions"  
The ad unit should always be unobstructed and within the defined size & aspect ratio. You may fix the size of the unit to a value that is within the bounds, and you may apply a border radius of up to 24px.
```




