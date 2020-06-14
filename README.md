# deep_portfolio_theory
Deep Portfolio Theory is a portfolio selection method published by J. B. Heaton, N. G. Polson, J. H. Witte from GreyMaths Inc.  Authors' codes are proprietary, We tried to implement this method on BSE Healthcare stocks. We constructed the deep portfolio method over the modern portfolio theory, Markowitz’s classic risk-return trade-off. Four-step routine of encode, calibrate, validate and verify to formulate an automated and general portfolio selection process. At the heart of our algorithm are deep hierarchical compositions of portfolios constructed in the encoding step. The calibration step then provides multivariate payouts in the form of deep hierarchical portfolios that are designed to target a variety of objective functions. The validate step trades-off the amount of regularization used in the encode and calibrate steps. The verification step uses a cross validation approach to trace out an ex post deep portfolio efficient frontier. We demonstrate all four steps of our portfolio theory numerically. 

Portfolio :- Collection of investment Tools such as stocks,bonds, mutual funds etc.

Portfolio management :- Manage to select the right investments for an individual to minimize their risk and maximize their return

Deep Portfolio Theory is a portfolio selection method build on Markowitz’s Classic Risk-return trade off using deep learning tools

Our Dataset Information
BSE Healthcare Stock & Index - Weekly basis
Current # of Stocks in BSE Healthcare =69
After Cleaning Data , # of Stocks in                                                                         BSE Healthcare we used = 48
Start-end Date = Jan 2012- dec 2016 
Training Data = jan 2012 - june 2015
Testing Data = june 2015 - dec 2016

Key Words - deep learning, hidden layers, autoencoder, artifical intelligence, activation function

Auto-encoding:

Train an auto-encoder model compressing market information.
Rank stocks by 2-norm difference then select subset of them as our portfolio. 
Leaky ReLU + linear as activation functions 
Weights 𝑊=(𝑊1,𝑊2) , L2 regularization

Lowest L2-norm ABBOT, P&G, REDDY, LUPIN,CIPLA
Highest L2-norm AJANTA, VIMTA, JUBLIANT, RPG,ALEMIC

For Building Portfolio we selected top 10  low L2-norm stocks +  Top X high L2-norm Stocks ,   X = {10 , 15 , 20, 25 , 35 }
 
Why? To balance the trade-off between risk and return as low L2-norm stocks are less risky so less return and high L2-norm stocks are more risky so more return

To reduce the effect of communal and non-communal information from both type of stocks on portfolio return and risk 
 
 



