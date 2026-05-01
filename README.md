# 5280 Collectibles - Image Assets Repository

This repository contains high-resolution images for Trading Card Game (TCG) inventory. These images are used as the primary source for the eBay Automation Suite.

## 📂 Organization

Images are organized by set or category:

- `pokemon151/`: Images for the Pokémon Scarlet & Violet 151 set.
- (Add more folders as sets are cataloged)

## 🖼️ Filename Standards

Images should be named following the pattern:
`[Set Number]-[Card Name].jpg`

Example:
- `01-Bulbasaur.jpg`
- `06-EX-Charizard.jpg`

## 🔗 Integration with eBay Automation

The `EbayAutomation` suite maps these images to the inventory CSV using the filename. The `update_csv.py` script in the `EbayAutomation/scripts` directory can be used to verify that every card in your manifest has a corresponding image in this repository.

## ⚠️ Usage Notes
- Avoid spaces in filenames where possible (though the system handles them).
- Use `.jpg` for the best balance of quality and file size for eBay listings.
- Ensure images are at least 500px on the longest side (eBay requirement).
