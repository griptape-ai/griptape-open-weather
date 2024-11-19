# Griptape OpenWeather Extension

## Overview
This extension provides a [Tool](https://docs.griptape.ai/stable/griptape-tools/) for [OpenWeather](https://openweathermap.org/).

```python
import os

from griptape.structures import Agent
from griptape.open_weather.tools import OpenWeatherTool

agent = Agent(
    tools=[
        OpenWeatherTool(
            api_key=os.environ["OPENWEATHER_API_KEY"],
        ),
    ]
)

agent.run("What's the weather currently like in San Francisco?")
```

## Installation

Poetry:
```bash
poetry add https://github.com/griptape-ai/griptape-open-weather.git
```

Pip:
```bash
pip install git+https://github.com/griptape-ai/griptape-open-weather.git
```

