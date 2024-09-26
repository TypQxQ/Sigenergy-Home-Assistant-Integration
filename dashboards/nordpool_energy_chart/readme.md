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
- Copy - paste the raw card codefrom `card_nordpool_energy_chart.yaml` to your a new card on you lovelace dashboard. Add any card and replace the raw code that you can edit by clicking on the *SHOW CODE EDITOR* in the bottom left.


# Configuration 

Configure your Nordpool integration.

In the chart-card you should change the following variables to suit your needs:

  - Check so the `nordpool_sensor:` name is correct.
  - The Grid import sensor name: `grid_import_sensor:`
  - Change `currency` if needed.
  - `chart_price_cutoff_coerficient` from 0 to 1 to show more or less barheight under the minimum value.
  - `decimals_in_prices` and `decimals_in_energy` to indicate how many decimals to show.
  - And any of the texts below.

If you use anything elsse than a Sigenergy system then change all values strating with sigen to suit your needs.

--

Happy savings!