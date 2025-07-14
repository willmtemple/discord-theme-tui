# discord-theme-tui

A TUI-inspired theme for BetterDiscord clients.

[Link to Theme File](https://raw.githubusercontent.com/willmtemple/discord-theme-tui/refs/heads/main/TUI-v0-BetterDiscord.theme.css)

**⚠️ NOTE**: This theme is an early work in progress, and I'm not incredibly good at CSS. If you have the skills to fix issues or theme remaining UI elements, please contribute them!

I've always wanted a full-featured discord client that has the minimal look and feel of a TUI and vibes with my [Hyprland](https://github.com/hyprwm/Hyprland) setup, so I decided to hack together a theme.

The design is heavily inspired by the amazing [Text theme for Spicetify](https://github.com/spicetify/spicetify-themes/blob/master/text/README.md).

## Screenshots

<img width="2037" height="1464" alt="image" src="https://github.com/user-attachments/assets/dfa0ee2e-4ff7-4376-a907-52d9411e390c" />

## Customizing

The theme has several variables that you can control:

```css
:root {
  /**
   * How to display the title bar.
   *
   * Valid values: none, block
   */
  --display-title-bar: none;

  /**
   * How much to push the top of the window up to account for the absence of the title bar.
   *
   * Set this to 32px if you had a title bar and set '--display-title-bar: none' to get rid of it. Otherwise, set it to zero.
   */
   --title-bar-v-offset: 32px;

  /**
   * How to display member activity.
   *
   * Valid values: none, block;
   */
  --display-member-activity: none;

   /**
    * How to display server banner images.
    *
    * Valid values: none, block;
    */
   --display-server-banner: block;

   /**
    * How much to push the server list down to account for the banner.
    *
    * Set this to 8em if you enabled server banners.
    */
   --server-banner-v-offset: 8em;

   /**
    * Primary font family. Used for most interface text except headers.
    */
   --font-primary: "Noto Sans Mono", monospace;

   /**
    * Default background color. This is lightened in some contexts for contrast.
    */
   --color-background: #121212;


   /**
    * Primary accent color.
    */
   --color-accent: #af2bdb;

   /**
    * An accent color to use for things that you're supposed to notice.
    *
    * - `@` mentioned message highlights.
    * - New message pill in channel/thread.
    */
   --color-accent-notice: #cc9322;

   /**
    * The accent color used for AV-related statuses (e.g. the mute/deafen icons, the "LIVE" status indicator).
    */
   --color-accent-av: #e50b2c;

   /**
    * Width between bordered panes in the UI.
    */
   --pane-gap-width: 20px;

   /**
    * Width of the pane borders.
    */
   --pane-border-width: 2px;

   /**
    * Primary border radius.
    */
   --pane-border-radius: 5px;

   /**
    * Subtle border radius (nested panes).
    */
   --pane-border-radius-subtle: 3px;

   /**
    * Time for mouse over transitions to apply. Set to 0 to disable.
    */
   --pane-transition-time: 0.2s;

   /**
    * Color used for the borders between panels.
    *
    * Default: 0x40 opacity white.
    */
   /*--color-panel-border: #ffffff40;*/

   /**
    * Color used for the title of panels.
    *
    * Default: 0x60 opacity white.
    */
   /*--color-panel-title: #ffffff60;*/

   /**
    * Color used for subtle borders (nested panels).
    *
    * Default: 0x30 opacity white.
    */
   /*--color-panel-border-subtle: #ffffff30 */
}
```

## Contributing

For fixes, please open a PR and include screenshots showing the before/after of your changes in the UI.

For design ideas, please open an issue describing what you think could be better.

## LICENSE

Licensed under the [MIT License](./LICENSE).

This project is not affiliated with Discord.
