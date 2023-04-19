# MapReduce Program to Find Maximum Temperature


![giphy](https://user-images.githubusercontent.com/88302656/233078709-159ac66d-0aaa-4a05-a033-91cb22d40ad3.gif)<br>
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

## Description

This repository contains a MapReduce program written in Java to find the maximum temperature from a given dataset. The program uses Hadoop MapReduce framework to process large amounts of data in parallel on a cluster of commodity hardware.<br>


## Table of Contents

- [Requirements](#requirements)
- [Input Format](#input-format)
- [Usage](#usage)
- [Output Format](#output-format)
- [Contact](#contact)

## Requirements

- Java 8 or higher
- Hadoop 2.7.1 or higher

## Input Format

The input dataset is assumed to be in the following format:<br>
![image](https://user-images.githubusercontent.com/88302656/233080255-f069c967-aa67-4efd-85f2-52a10e100668.png)<br>


where `station_name` is a string representing the name of the weather station, `year` is a string representing the year in `yyyy` format, and `max temperature` is a float representing the temperature in Fahrenheit.

## Usage

To run the MapReduce program, you need to first create a jar file using the following command:

This will create a `mapreduce-1.0-SNAPSHOT.jar` file in the `home` directory. You can then run the program using the following command:

$ hadoop jar home/mt.jar MaxTemperature <input_path> <output_path>

where `<input_path>` is the path to the input dataset and `<output_path>` is the path to the output directory where the maximum temperature will be written.

## Output Format

The output of the program is a single line containing the maximum temperature and the date on which it occurred. The output is in the following format:
![image](https://user-images.githubusercontent.com/88302656/233081230-df1f3cbf-13d0-4aa4-a0c6-1a2d36583525.png)


## Contact

If you have any questions or suggestions, please feel free to connect with us.



