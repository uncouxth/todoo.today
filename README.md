<img src="https://todaylist.io/assets/images/icon.png" width="128" height="128">

# <a href="https://www.todoo.today/">todoo.today</a> a minimal 24 hour todo list app

A todo list to help you organize your day ahead. <a href="https://github.com/daniel-hayes/today">Based on Today v1.4 by Daniel Hayes.</a>

**Visit** <a href="https://www.todoo.today/">todoo.today</a> and try it yourself! 100% free forever. (not yet)

<br>

## Todos

**v0:** First port with better usability
- **Keep Ups** &rarr; Carry over uncompleted tasks
- **List Groups** &rarr; Make sublists for related tasks
- **Task Intervals** &rarr; Place a timebox around a task
- **Keep Momentum** &rarr; Hide completed tasks

**v1:** Visual & UX considerations 
- **It's Alive!** &rarr; Snazzy new animations
- **Paint it Black** &rarr; Better color selection
- **Enhance. ENHANCE.** &rarr; Multiple display widths
- **Persistent Focuses** &rarr; Idea bait for the start of the day

> The list clears every 24 hours which will allow you to focus on your daily tasks without letting them pile up.


### Today - Desktop App

#### Built with Svelte + Electron + Typescript

<div>
  <img src="https://todaylist.io/assets/images/light.png" width="49%">
  <img src="https://todaylist.io/assets/images/settings.png" width="49%">
</div>

## Development

```
yarn install
```

Run locally in watch mode:

```
# From root
yarn workspace @today/desktop start

# From /packages/desktop
yarn start
```

Build app:

```
# From root
yarn workspace @today/desktop build # or `build:prod`

# From /packages/desktop
yarn build # or `build:prod`
```

### Today - iOS App

#### Built with Svelte + Capacitor + Typescript

```
yarn install
```

Run locally in watch mode:

```
# From root
yarn workspace @today/mobile dev:ios

# From /packages/mobile
yarn dev:ios
```

Build app:

```
# From root
yarn workspace @today/mobile build:ios

# From /packages/mobile
yarn build:ios
```

#### Custom themes

You can add a new theme to the [themes.json](https://github.com/daniel-hayes/today/blob/main/packages/shared/themes/themes.json) file. Each new theme requires the following fields:

```
  {
    "title": "My Theme",
    "file": "my-theme.css",
    "primary": "#5dbbea",
    "secondary": "#f0f0f0",
    "accent": "#5dbbea"
  }
```

NOTE: These should be added in alphabetical order (A-Z) based on the title of the theme.

After adding your theme to the themes.json config, you can run:

```
npm run generate:css
```

This will create the CSS files associated with your theme. They will then automatically be accessible in the theme menu.

## Download

<a href="https://github.com/daniel-hayes/today/releases">
  Releases
</a>
