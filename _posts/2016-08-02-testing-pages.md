---
layout: post
title: PUBG Finish Placement Prediction
author: Chenlu Wang
date: 2019-08-02
---




## Abstract
-----

The project is mainly based on the dataset of game Player Unknown’s Battle Ground. PUBG is a player versus player shooter game in which up to 100 players start in each match and they can be on teams which get ranked at the end of the game based on how many other teams are still alive when they are eliminated. In game, players can pick up different munitions, revive downed-but-not-out (knocked) teammates, drive vehicles, swim, run, shoot, and experience all of the consequences -- such as falling too far or running themselves over and eliminating themselves.

This project uses ideas of machine learning based on logistic regression, random forest and xgboost for fitting and prediction. The goal is to use dataset given through Kaggle to predict the target variable and have ideal error based on mean squared error loss function. The result of this project is provided by xgboost model with 0.02 mse.

## 1.Introduction
-----

PlayerUnknown's  BattleGrounds  (PUBG)  is  an  online  multiplayer  battle  game developed and published by PUBG Corporation, a subsidiary of South Korean video game  company  Bluehole.  The gameis  based  on  previous  mods  that  were  created  by Brendan "PlayerUnknown" Greene for other games, inspired by the 2000 Japanese film Battle Royale, and expanded into a standalone game under Greene's creative direction. In  the  game,  up  to  one  hundred  players parachute  onto  an  island  and  scavenge  for weapons  and  equipment  to  kill  others  while  avoiding  getting  killed  themselves.  The available safe area of the game's map decreases in size over time, directing surviving players into tighter areas to force encounters. The last player or team standing wins the round.

## 2. Exploratory Data Analysis
-----

### 2.1 summary
-----

The dataset is made up of 29 variables with size 29*4446966. All variables can be grouped into three different classes. First class consists variables showing the information of matching and type of games, like groupID which shows members in different groups and matchType showing whether player played the game alone or with others. Second class consists variables about performance of the players, like headshotKills which shows how many enemies player eliminated by directly shooting
the head and teamkills which is the number of times this player killed a teammate. The last class are variables describing the rank of players, like winPlacePerc which is the percentile winning placement and rankPoints, which shows Elo-like ranking of players.


<table>
   <tr>
      <td colspan="3"> <center> Classification of Variables </center> </td>
   </tr>
   <tr>
      <td>  <center> Game type information <center> <td>  Gaming behavior  <td> <center> Rank information  </td>
   </tr>
   <tr>
      <td> <center> groupID <td> <center> Assists, heals,revives  <td> <center> killPlace </td>
   </tr>
   <tr>
      <td>  <center> Game type information <td> <center> Gaming behavior  <td>  <center> Rank information  </td>
   </tr>
</table>



![avatar](/picture/1.png)
