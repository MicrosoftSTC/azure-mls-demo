# Azure Machine Learning Studio Demo

This project contains demo for studuj.digital live event.

## Goals of the project
 1. Create Azure ML Studio project which predicts price of laptop by some hardware parameters.
 2. Create console application written in Kotlin which sends HTTP Post request to Azure ML Studio Web Service and recieves predicted price of laptop.

## Dataset
The Laptop price data set by Karl Tillström, 2020
Source: [https://www.machinelearningfordevelopers.com/datasets/laptopprices](https://www.machinelearningfordevelopers.com/datasets/laptopprices)

## Requirements

 - Basic understanding of [Kotlin programming language](https://kotlinlang.org/)
 - [studuj.digital Live Demo](https://gallery.cortanaintelligence.com/Experiment/studuj-digital-Live-demo) experiement cloned in your Azure ML Studio

## Setup
 - Clone repository.
 - Add URL of Web Service (at bottom of MainKt).
 - Add API token (at bottom of MainKt).
 
```kotlin
/**
 * Azure ML Studio > Web Service > HTTP Request/Response > URL
 * */
const val azureUrl =
    "<url of your web service>"

/**
 * Azure ML Studio > Web Service > API token
 * */
const val apiToken = "<your api token>"
```

## Used
### Software
 - [Azure Machine Learning Studio](https://studio.azureml.net/) (for machine learning and as a back-end for console app)
 - [JetBrains IntelliJ IDEA](https://www.jetbrains.com/idea/) (for programming of console app)

### Libraries

 - [KotlinX Serialization](https://github.com/Kotlin/kotlinx.serialization) (for JSON (de)serialization)
 - [KotlinX Coroutines](https://github.com/Kotlin/kotlinx.coroutines) (for handling HTTP await thread)
 - [Fuel](https://github.com/kittinunf/fuel) (for HTTP networking)


## More Resources
You can find more info about how to use Azure Machine Learning Studio (Classic) in [AI series with 6 articles at STC blog](https://studuj.digital/2020/03/19/umela-inteligence-predstaveni/).
