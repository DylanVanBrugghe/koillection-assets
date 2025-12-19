# Koillection Assets
A small collection of assets and scraper configurations used with my personal Koillection instance.

## Table of contents
- [Collection images](#collection-images)
- [Scraper configurations](#scraper-configurations)
- [Contributing](#contributing)
- [Attribution](#attribution)

## Collection images
The [`collection-images`](collection-images) folder contains the images and source assets used for collections, plus an editable Photoshop template.

**Folder structure:**
- [`collection-images/template.psd`](collection-images/template.psd) — editable template
- [`collection-images/*.md`](collection-images/) — attribution files for sources requiring attribution
- [`collection-images/`](collection-images/) (root) — 200×200 PNG images registered/used in Koillection
- [`collection-images/source/`](collection-images/source/) — original/source files (SVG, high-resolution images, logos, and variants)

## Scraper configurations
Scraper configurations are stored in the [`scrapers`](scrapers) folder. Import the JSON files using Koillection's import feature, or manually create the scraper using the Koillection web UI.

- [Amiibo](scrapers/amiibo)
  - [amiibo life](https://amiibo.life/): [`scrapers/amiibo/amiibo-life.json`](scrapers/amiibo/amiibo-life.json)
- [Funko](`scrapers/funko`)
  - [POP's Today](https://pops.today/): [`scrapers/funko/pop-s-today.json`](scrapers/funko/pop-s-today.json)
- [LEGO](scrapers/lego)
  - [LEGO](https://lego.com/): [`scrapers/lego/lego-com.json`](scrapers/lego/lego-com.json)
- [MEGA](scrapers/mega)
  - [Mattel (US)](https://shop.mattel.com/): [`scrapers/mega/mattel-us.json`](scrapers/mega/mattel-us.json)
  - [Mattel (EU)](https://shopping.mattel.com/): [`scrapers/mega/mattel-eu.json`](scrapers/mega/mattel-eu.json)

## Contributing
Contributions are welcome! Please open a pull request with a clear description of what you're adding and the data source.

**Adding collection images:**
1. Edit [`template.psd`](collection-images/template.psd) using your source image
2. Export a 200×200 PNG to the [`collection-images/`](collection-images/) root
3. Save the source image to [`collection-images/source/`](collection-images/source/)
4. If attribution is required, update the appropriate attribution file in [`collection-images/`](collection-images/) (e.g., [`flaticon-attribution.md`](collection-images/flaticon-attribution.md)) or create a new one for other sources

**Important:** When adding new scraper configurations, you must also update the ["Scraper configurations"](#scraper-configurations) section in this README. Follow the existing format:

```
- <category1>
  - <website1>: <path1>
  - <website2>: <path2>
- <category2>
  - <website3>: <path3>
```

This ensures all configurations are documented and easy to find.
**Adding scraper configurations:**
1. Add the configuration JSON file in [`scrapers/<category>/`](scrapers/)
2. Include the data source in your pull request description

## Attribution
- [Flaticon icons](collection-images/flaticon-attribution.md)