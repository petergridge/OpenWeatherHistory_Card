# Custom Card for OpenWeatherHistory Component<img src="https://github.com/petergridge/irrigation_card/blob/main/icon.png" alt="drawing" width="75"/>

## Installation
HACS installation
* Will be available on HACS soon but you can add it a custom repository.

Manual install
* Ensure you have advanced mode enabled in Home Assistant
* Copy openweatherhistory-card.js to the /config/www directory in Home Assistant
* In the *configuration/LoveLace* dashboards page select the *Resources* tab
* Add the resource */local/openweatherhistory-card.js?v=1* increment the version number if updating an exsting installation
* Add a manual card with the definition below

## Configuration

**type:** (required) custom:open-weather-map-history-card

**entity_id:** (required) The openweatherhistory sensor

**title:** (optional) The title to be set in the card. defaults to the program freindly name

**icon:** (optional) An icon to display to the left of the title.

**theme:** (optional) Override the used theme for this card with any loaded theme. For more information about themes, see the [frontend documentation](https://www.home-assistant.io/integrations/frontend/).

**header:** (optional) Header widget to render an image. See [header/footer documentation](https://www.home-assistant.io/lovelace/header-footer/).

**footer:** (optional) Header widget to render and image. See [header/footer documentation](https://www.home-assistant.io/lovelace/header-footer/).

**Example:**
```yaml
type: custom:open-weather-map-history-card
entity_id: sensor.rainfactor
```

## REVISION HISTORY

### 1.0.0
* New repository
