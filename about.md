---
layout: article
titles:
  # @start locale config
  en      : &EN       About
  en-GB   : *EN
  en-US   : *EN
  en-CA   : *EN
  en-AU   : *EN
  zh-Hans : &ZH_HANS  关于
  zh      : *ZH_HANS
  zh-CN   : *ZH_HANS
  zh-SG   : *ZH_HANS
  zh-Hant : &ZH_HANT  關於
  zh-TW   : *ZH_HANT
  zh-HK   : *ZH_HANT
  ko      : &KO       소개
  ko-KR   : *KO
  fr      : &FR       À propos
  fr-BE   : *FR
  fr-CA   : *FR
  fr-CH   : *FR
  fr-FR   : *FR
  fr-LU   : *FR
  # @end locale config
key: page-about
---

![SPADE DEMO](https://raw.githubusercontent.com/tamagusko/spade/main/screenshots/spade_app.png)

Our SPADE project is all about helping cities stay ahead of flooding. We analyze elevation models, road data, and satellite images to figure out where water might flow and which areas are most at risk. This information can then be used to improve urban design and prevent flooding. It's all about using smart data to keep cities safe and dry!

## Concept

The project aims to solve the problem of flooding in smart cities. The team uses location-based data, the Digital Terrain Model (DTM), and satellite images to predict water flow paths and areas vulnerable to floods. This information creates a map that displays flooded areas and safe routes for rescue efforts. The map has a scroll bar that shows how flooding changes with different rainfall amounts. The team creates a point cloud of city elevations from the Digital Terrain Model and calculates water flow and waterways using algorithms. A satellite image segmentation algorithm estimates the permeability of each region and identifies existing water courses for drainage. The team then uses routing algorithms to avoid flood-prone areas and updates the city's situation and available roads based on the amount of rain. The project results in a real-time system that provides information about flooded areas and safe routes during a flood event, accessible through a user-friendly interface, like a web-based map, updated in real-time with new information.

### Goals

1. Attribute drainage coefficients to areas through satellite images: Applying a neural network, be capable of classifying the surface cover of an area and estimate the volume of rain that it can absorb.
2. Define possible flood areas and water flow paths: Through Digital Elevation Model (DEM) files, define basins, and higher and lower points of the city, as long as the path of rainwater from the higher to the lower ground.
3. Identify the impact on roads and general transport infrastructure: Goals 1 and 2 will provide the necessary data for estimating which areas are in danger of flood and which roads can become unable to drive. This knowledge can be used to design alternative rescue routes together with adjustments in the existing transport.

## Features

- Areas analyzed classified into three classes: City (black), Vegetation (green), Water (blue).
- Real-time flood prediction using location-based data and weather information
- Safe route planning for rescue efforts during floods
- User-friendly map interface displaying flooded areas and safe routes

## MVP

[spade-hackathon.streamlit.app](https://spade-hackathon.streamlit.app/)
