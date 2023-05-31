# EBN frontend
## Note:
Please do not edit de.json, fr.json and nl.json locally as them will be replaced by files from crowdin
## Setup

Install the dependencies:

```bash
# yarn
yarn install

# npm
npm install
```

Recommended to setup local virtualhost (http://ebn.local:3000)

## Development Server

Start the development server on http://localhost:3000

```bash
yarn dev
```

## Build the application:

```bash
#development
yarn build

#staging
yarn build:staging

#production
yarn build:production
```

# Preview generated build:

```bash
npm run preview
```

## Default folders structure:

```
/composables, /env, /layouts, /pages, /utils, /public - needs no introduction

/assets - for images, icons, css files(like reset.css), global scss variables etc.

/components - for global-used components like header, footer, slider or ui/ux components like icons or customizable buttons

/const - will be fine to store here enums and something like route-names.const.ts

/models - keep here global models only, like user.model.ts, error.model.ts etc.

/repositories - for api repositories. An AuthModule created for example

/modules - should contain only module-specific files and nested folders structure like:
    /cart
        /components
            CartSection.vue
            CartItem.vue
            ...
        /models
            cart-item.model.ts
            ...
        /const
            product-type.enum.ts
            ...
        ...
    ...
```

