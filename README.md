# PyThalesians

PyThalesians is a Python financial library developed by the Thalesians (http://www.thalesians.com). Whilst elements of 
the project will remain proprietary (such as our proprietary trading algorithms), we are keen to publish many of the 
more generic elements to the community, many of whom have encouraged me to publish my code.

At present the open source version (0.1a) of PyThalesians offers:
* Seamless historic data downloading from Bloomberg (requires licence), Yahoo, Quandl and other market data sources
* Produces beautiful line plots with PyThalesians wrapper (via Matplotlib) and a simple wrapper for Bokeh
* Helper functions built on top of Pandas
* Automatic tweeting of charts
* And much more!
* Please bear in mind at present PyThalesians currently a highly experimental alpha project and isn't yet fully 
documented
* Uses Apache 2.0 licence

The proprietary version of PyThalesians also has:

* Backtesting systematic trading strategies for cash markets
* Analysis of intraday price action around data events
* Comprehensive number crunching of FX volatility market around data events
* Seasonality analysis of markets
* Backtesting systematic trading strategies in FX vanilla options
* Implemented a trading signals based on a number of technical indicators
* Elegant caching framework for historical market data
* Proprietary trading algorithms used in my own personal trading

# Gallery

Below we give some examples of analysis which we've done using the full code of PyThalesians (which currently includes more features than the open source version).

<img src="https://raw.github.com/thalesians/pythalesians/master/examples/usdjpy-nfp-delta.png" width="543"/>

*Using PyThalesians to plot & calculate USD/JPY intraday moves around non-farm payrolls over past 10 years*

<img src="https://raw.github.com/thalesians/pythalesians/master/examples/fx-intraday-vol.png" width="543"/>

*Using PyThalesians to calculate intraday vol in major FX crosses by time of day*

<img src="https://raw.github.com/thalesians/pythalesians/master/examples/replicating-cta.png" width="543"/>

*Using PyThalesians to create the Thalesians CTA index (trend following), which replicates Newedge CTA index benchmark*

# Requirements

PyThalesians has been tested on Windows 8 running Bloomberg terminal software. Potentially, it could also work on the 
Bloomberg Server API (but I have not explicitly tested this).

Major requirements
* Python 3.4+
* pandas, matplotlib etc.
* Recommended: Bloomberg Python Open API (use Python 3 version from https://github.com/filmackay/blpapi-py/) or 
alternatively to access Bloomberg, the software also supports the old COM API
* To use Bloomberg you will need to have a installed licence

# Installation

After installing manually, please make sure you edit pythalesians.util.constants for the following variables:
* Change the root path variable - this will ensure that the logging (and a number of other features works correctly). 
Failure to do so will result in the project not starting
* Change the default Bloomberg settings (Which API to use? What address to use?
* Planning to have installation via pip

# About the Thalesians

The Thalesians are a think tank of dedicated professionals with an interest in quantitative finance, economics, 
mathematics, physics and computer science, not necessarily in that order. We run quant finance events in London, New York,
Budapest, Prague and Frankfurt (join our Meetup.com group at http://events.thalesians.com). We also publish research
on systematic trading and also consult in the area. One of our clients is RavenPack, a major news analytics vendor.

# Supporting PyThalesians project

If you find PyThalesians useful (and in particular if you are commercial company) please consider supporting the project
through sponsorship or by using our consultancy/research services in systematic trading.

For the UK election Plot.ly code - please visit https://github.com/plotly/IPython-plotly/tree/master/notebooks/ukelectionbbg

Saeed Amen (managing director & co-founder of the Thalesians)

# Future Plans for PyThalesians

We plan to add the following features:
* Have a proper setup mechanism (eg. via pip), at present needs manual deployment
* Add Plotly & Seaborn wrappers for plotting
* Improve support for Bokeh plotting
* Add more plots from Matlibplot
* Add Reuters as a historic data source
* Add ability to stream data from Bloomberg and Reuters
* Use event driven code to generate trading signals (to be used live and historically)
* Integrate support for zipline as an alternative trading system
* Support Python 2.7+

More generally, we want to:
* Make existing code more robust
* Increase documentation and examples

# Release Notes

* 0.1a (highly experimental alpha version)
* Basic implementation of plotting for line charts
* Basic downloading of market data like Bloomberg/Yahoo etc. via generic wrapper

End of note
