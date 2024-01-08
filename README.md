# Undergraduate Dissertation - 递归神经网络时间序列预测 / Recurrent Neural Networks for Time Series Forecasting (Exchange rate Between the Japanese Yen and US Dollar)

## Introduction / 介绍

This repository contains a portion of the data and code from my personal graduation thesis. My research focuses on exploring the performance of different Recurrent Neural Networks (RNNs) applied to time series data, particularly in the context of predicting exchange rates.

这个仓库包含了我的个人毕业论文的一部分数据和代码。我的研究致力于探讨在时间序列数据（特别是汇率数据）预测中应用不同的递归神经网络（Recurrent Neural Networks，RNNs）的性能。

## Abstract / 论文摘要

To study whether recurrent neural networks are suitable for constructing short-term exchange rate prediction models based on traditional economic theories, the main focus of this article is as follows:

为了研究递归神经网络是否适用于基于传统经济理论构建短期汇率预测模型，本文的主要关注点如下：

I) Employ RNNs, LSTM, BILSTM, and other Recurrent Neural Networks to build short-term exchange rate forecasting models based on Uncovered Interest Rate Parity (UIRP), Purchasing Power Parity (PPP), the Monetary model, and the Taylor Rule model, which are four classic economic theories.

I) 使用RNNs、LSTM、BILSTM等递归神经网络构建基于无遮蔽利率平价（UIRP）、购买力平价（PPP）、货币模型和泰勒规则模型的短期汇率预测模型，这四个是经济学中的经典理论。

II) Compare the neural network prediction models with and without additional economic variables under classic economic theories, to measure the predictive effect of these models and analyze the underlying reasons.

II) 在经典经济理论下，比较具有和不具有额外经济变量的神经网络预测模型，以衡量这些模型的预测效果并分析其根本原因。

III) Construct an ARIMA-Stacked LSTM Hybrid model based on ARIMA and LSTMs to achieve more accurate exchange rate predictions with the comparison of Random Walk.

III) 基于ARIMA和LSTMs构建ARIMA-Stacked LSTM混合模型，通过与随机游走的比较实现更准确的汇率预测。

## Dataset / 数据集

The data for this paper comes from the OECD and each country's respective National Data Providers. Specifically, the Producer Price Index (PPI) and JPY/USD exchange rate for the United States and Japan are sourced from FRED and BOJ. Other data used includes each country's Monetary Aggregate-Narrow money (M1), which represents monetary demands, the Industrial Production Index (IPI), representing the output of both economies (as GDP is only calculated quarterly). Additionally, the bond yields of both countries, including Immediate/Short-term/Long-term yields used to indicate interest rates, are sourced from the OECD.

本文的数据来源于OECD和各国的国家数据提供机构。具体而言，来自FRED和BOJ的生产者物价指数（PPI）和美元/日元汇率用于美国和日本。其他使用的数据包括每个国家的货币聚合-狭义货币（M1），代表货币需求，工业生产指数（IPI），代表两个经济体的产出（因为GDP仅按季度计算）。此外，包括用于表示利率的两国的债券收益率，包括即期/短期/长期收益率，这些数据均来自OECD。

The analysis methodology utilizes a rolling windows analysis methodology to conduct one-period forecasts using a monthly dataset spanning from January 1980 to March 2023.

分析方法采用滚动窗口分析方法，使用从1980年1月到2023年3月的月度数据集进行单期预测。



## Notes / 注意事项

- Ensure that you have installed the required dependencies and packages before running the code. The following packages are essential for the successful execution of the project:

  Python 3.10.9
  Numpy (Van Der Walt et al., 2011)
  Pandas (McKinney, 2010)
  Matplotlib (Hunter, JD, 2007)
  SciPy (Jones, E. et al, 2001)
  Scikit-Learn (Pedregosa et al., 2011)
  Keras
  TensorFlow (Abadi et al., 2016)
- Ensure that the required dependencies are installed.
- Some code may need adjustment based on your specific requirements.

- 请确保已经安装了所需的环境以及packages。
- 部分代码可能需要根据你的具体情况进行调整。

## Feedback and Contributions / 反馈与贡献

Feedback and suggestions are welcome. If you find any issues or wish to contribute, please raise an issue or submit a pull request on GitHub.

欢迎提供反馈和建议。如果你发现了问题或想要做出贡献，请在 GitHub 上提出问题或发送拉取请求。

Thank you for your interest in my research! 感谢你对我的研究的关注！
