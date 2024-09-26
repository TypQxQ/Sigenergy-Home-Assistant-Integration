# Energy price chart using nordpool prices.

This is my atempt at a chart displaying todays prices and tomorows prices when available along with imported energy.
- Upper and Lower price threshold is calculated for today+tomorows ***comming*** price.
  - Orange is upper 3:rd of the pricing interval.
  - Green is lower 3:rd of the prices interval.
  - Red is the upper 10% of the pricing interval.

![alt text](HA_energy_chart.jpg)

# Pre-requirements

This has not been tested on HA earlier than 2024.9 and requires the following HACS addons:

- Nordpool - For getting energy prices.
- Apex-Charts card
- Config Template Card Card - For scripting inside the chart card.
- lovelace-card-mod - For styling.

The Nordpool entity should be changed from the default name to just "nordpool" as per the components installation instructions.

# Installation
- Add the `nordpool_energy_chart.yaml` file to Home Assistant's packages folder for inclusion in Home Assistant. See here for example: [Installation of Sigenergy integration](https://github.com/TypQxQ/Sigenergy-Home-Assistant-Integration/wiki/2.-How%E2%80%90to%E2%80%90install)
- Copy - paste the raw card codefrom `card_nordpool_energy_chart.yaml` to your a new card on you lovelace dashboard. Add any card and replace the raw code that you can edit by clicking on the *SHOW CODE EDITOR* in the bottom left.


# Configuration 

Configure your Nordpool integration.

In the chart-card you should change the following variables to suit your needs:

  - Check the `nordpool_sensor` name is correct.
  - The Grid import sensor name: `grid_import_sensor`
  - `chart_cutoff` to what you want the minimum in the chart to be. I have to pay at least 0.7 SEK in grid transfer fee.
  - `currency` to whatever currency you want.
  - `decimals_in_prices` and `decimals_in_energy` to indicate how many decimals to show.

If you use anything elsse than a Sigenergy system then change all values strating with sigen to suit your needs.

--

Happy savings!