# W5100S-Pico-Electric-Cushion

![image](https://github.com/wiznetmaker/W5100S-Pico-Electric-Cushion/assets/111826791/3ef59757-7a08-4114-8bc5-c406eddc5cc2)

My butt was always cold.What if AI always sets my butt to the right temperature.I'll be able to concentrate on my work without having to wear it on my butt.

![image](https://github.com/wiznetmaker/W5100S-Pico-Electric-Cushion/assets/111826791/c9cc0ef9-a212-4fc0-9597-90d8e593067f)

## Hardware

The main board is the Raspberry Pi Pico. I used the W5100S PoE board that we worked on for Ethernet communication. The PoE board can receive up to 10 W of power.

![image](https://github.com/wiznetmaker/W5100S-Pico-Electric-Cushion/assets/111826791/0edbb5b8-ed98-485a-ae19-f8c79791af06)

I used FET to send 10W of output to resistance. It's not a big power, so I brought a nearby FET and used it. As you can see, we also have damping resistance.

![image](https://github.com/wiznetmaker/W5100S-Pico-Electric-Cushion/assets/111826791/43bf19b1-883c-49af-bd03-c31013486fa1)

First of all, we tested by connecting 4 20 ohm resistors in parallel.When I printed out 5W, I found that the resistance was very hot.

![image](https://github.com/wiznetmaker/W5100S-Pico-Electric-Cushion/assets/111826791/2ea23023-e363-4f37-b341-f6319b5cf386)

Now it's the sitting mat's turn. At first, I was going to repair the cushion and put resistance in it. But the cushion didn't give up his belly so easily.

![image](https://github.com/wiznetmaker/W5100S-Pico-Electric-Cushion/assets/111826791/98d9c44b-e66a-4d7e-9fa6-8741af602487)

Eventually, I put the resistance on the chair, and I put the cushion on it.

## Firmware

![image](https://github.com/wiznetmaker/W5100S-Pico-Electric-Cushion/assets/111826791/6a80c165-0beb-4cc7-ba89-406e6c5ef827)

https://www.hackster.io/alan43/wow-enjoy-the-current-weather-with-picasso-s-painting-1e01f4
The basics are as shown in the project below.
In this project, you only need to get the expected weather information through Web Crawling.

![image](https://github.com/wiznetmaker/W5100S-Pico-Electric-Cushion/assets/111826791/b0dafc2f-f25f-4cda-8e43-48132e036277)

https://www.hackster.io/alan43/chat-gpt-api-youtube-comment-weather-2e03bb
The firmware was taken from the project above.

### Web Crawling

GPT does not currently support real-time data services. So I decided to read it on Naver as WebCrawling.It started implementing in a Python environment that is relatively light and easy to implement.

![image](https://github.com/wiznetmaker/W5100S-Pico-Electric-Cushion/assets/111826791/19428eb5-5784-4add-8e22-c5a2e59e3411)

WebCrawling can be done simply with a package called BeautifulSoup.

![image](https://github.com/wiznetmaker/W5100S-Pico-Electric-Cushion/assets/111826791/27587015-fdc2-4dce-9a9a-8b0208b731ba)

<Screen that appears when searching for weather in the water on the Naver site>
Let me deal with Crawling briefly.

![image](https://github.com/wiznetmaker/W5100S-Pico-Electric-Cushion/assets/111826791/89508989-f6d3-474a-9299-cea19d899201)

In the script, temperature was read from temperature_text.

![image](https://github.com/wiznetmaker/W5100S-Pico-Electric-Cushion/assets/111826791/9647c7a7-9566-4420-a791-4f5239b5d39c)

And weather was read in the span class of weather before_slash.

![image](https://github.com/wiznetmaker/W5100S-Pico-Electric-Cushion/assets/111826791/ef27b3ec-c2b0-4621-a156-92b6e6916851)

I want to read it in English, but I couldn't find it, so I just hardcoded it...And when you run this, it will look like the following.

![image](https://github.com/wiznetmaker/W5100S-Pico-Electric-Cushion/assets/111826791/2785b8ac-8be9-42a7-a600-edac2694f3bc)

It outputs temperature and weather like this.

## Operating

![image](https://github.com/wiznetmaker/W5100S-Pico-Electric-Cushion/assets/111826791/85d29b42-06d0-4c4e-81b3-ed9b31756994)

The temperature does not rise under very hot temperatures.

![image](https://github.com/wiznetmaker/W5100S-Pico-Electric-Cushion/assets/111826791/b6121a38-4e20-4ea1-87b5-4603bf768ebc)

Moderate spring weather? The temperature goes up a little bit. Actually, I think it'll be hot if it goes up to here. I need to fix it!

![image](https://github.com/wiznetmaker/W5100S-Pico-Electric-Cushion/assets/111826791/c35a0944-12e1-4da1-887b-c21d1be8ae4e)

I set it to very cold weather. The temperature rises to 65.7 degrees. My butt will be warm!

![image](https://github.com/wiznetmaker/W5100S-Pico-Electric-Cushion/assets/111826791/045c546b-ca5c-4aac-9acc-fe3df601ad27)

It's getting colder... The picture explains the weather outside. It looks so cold!

![image](https://github.com/wiznetmaker/W5100S-Pico-Electric-Cushion/assets/111826791/c9a9a5c3-cc3a-43de-a5be-67dff8d4fe0d)

There's a problem! Even if it gets colder, it should be moderately hot! If it snows a lot, my butt will burn!

## Review 

![image](https://github.com/wiznetmaker/W5100S-Pico-Electric-Cushion/assets/111826791/af3c41eb-0855-4e54-8a02-7dce71e020c4)

I'm using it well, but our company has a heater... If it's cold outside and the office is hot, there's a problem..











