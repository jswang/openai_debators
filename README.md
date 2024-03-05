# OpenAI Debators

![Alt Text](docs/city_hall.jpeg)

Are you trying to be an informed voter? Do you hate listening to talking heads attack each other and never talk about the actual issues? Do you just want to know what the measures are and then here intelligent debate around them? 

Well this repo is for you! We feed the [official city election guide](https://voterguide.sfelections.org/local-ballot-measures) from San Francisco for the upcoming 2024 city ballot measures to the [OpenAI Assistants API](https://platform.openai.com/docs/api-reference/assistants), then create both an audio recording using [OpenAI's TTS model](https://platform.openai.com/docs/models/tts). 

The result? High quality, informed debate on all 7 measures up for election this year.
You can adjust the number of rounds, each debator will open and close their debate.  Worried about me trying to sway you to either side? This repo open sources the instructions given to each agent, so you can examine exactly what they are asked to do. 

Enjoy!

## Results
[Measure A: Housing Bonds](https://voterguide.sfelections.org/local-ballot-measures/measure-a)

### Audio

### Text
Full text [here](docs/measure_a.txt)
<br>
Snippet:
> Moderator: Please concisely summarize Measure a and your stance on it
<br><br>
Debater for Measure a: <br><br>
Measure A, known as the San Francisco Affordable Housing Bonds, aims to address the critical issue of housing affordability in San Francisco by authorizing the city to issue $300 million in general obligation bonds. These funds would be used to construct, develop, acquire, and rehabilitate housing that will be affordable for households ranging from extremely low-income to moderate-income, including specific provisions for workforce and senior housing. <br>
As a supporter of Measure A, I believe this initiative is a necessary and significant step towards ensuring that diverse populations, including firefighters, teachers, nurses, veterans, families, and seniors, can continue to afford to live in San Francisco. This measure not only promotes social equity by providing affordable housing opportunities but also contributes to the stability and sustainability of the community by supporting those who serve it.
<br><br>
Debater against Measure a:
<br><br>
I firmly stand against Measure A, the San Francisco Affordable Housing Bonds proposal, because while its intention to provide affordable housing seems noble, it comes with significant tax implications and potential for inefficient use of taxpayer money. Furthermore, it may not effectively address the underlying issues of housing affordability and could result in unforeseen consequences that exacerbate the problem. As an opponent, I question the transparency and accountability measures in place to ensure that these funds will be used efficiently and prioritize those most in need. It's essential to consider alternative solutions that do not place an additional tax burden on property owners and potentially renters, who may see a pass-through of these costs.


## Setup
1. Generate an OpenAI key: https://platform.openai.com/api-keys. 
2. Export it to your local environment using `export OPENAI_API_KEY=<your key here>`
3. Launch the included jupyter notebook and run the cells. 
4. Output will be place in `<location of repo>/outputs`