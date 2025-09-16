# Weather Data Storage System

## Overview

Stores temperature data indexed by **(year, city)** using both **dense 2D arrays** and **sparse dictionaries**.

## Components

* **WeatherRecord ADT**: `(date, city, temperature)`
* **Storage**:

  * Dense: `table[year][city]` with `NaN` for missing.
  * Sparse: `{(year, city): temp}`

## Methods

* `insert(year, city, temp)`
* `delete(year, city)`
* `retrieve(year, city)`
* `row_major_access()` / `column_major_access()`
* `to_sparse()`

## Usage

* Dense: good for full data.
* Sparse: efficient for missing data.

