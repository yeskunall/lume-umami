# lume-umami

<!-- deno-fmt-ignore-start -->

> A [Lume plugin](https://lume.land/docs/configuration/install-plugins/) to add [Umami Analytics](https://umami.is/) to your website.

<!-- deno-fmt-ignore-end -->

## 🪶 Highlights

- Disables events and pageviews during development
- Prevents Google Tag Manager from stripping custom `data-*` attributes
- Supports all [configuration](https://umami.is/docs/tracker-configuration) options
- (_Optionally_) Serve the tracking script using [Partytown](https://partytown.builder.io/) (_**planned in an upcoming release**_)
- **Actively maintained**

## 🍛 Usage

### Install

1. Install the required dependencies

```sh
deno add jsr:@yeskunall/lume-umami
```

2. Add the integration to your Lume config:

```diff
import lume from "lume/mod.ts";
+ import umami from "jsr:@yeskunall/lume-umami";

const site = lume({});

+ site.use(umami({ id: "94db1cb1-74f4-4a40-ad6c-962362670409" }));
```

###### 📖 For all configurable options, see the [interface](https://github.com/yeskunall/lume-umami/blob/main/mod.ts#L11).

---

#### ⚖️ License

<!-- deno-fmt-ignore-start -->

[MIT](https://github.com/yeskunall/lume_umami/blob/main/license) © [Kunall Banerjee](https://kunall.dev/)

<!-- deno-fmt-ignore-end -->
