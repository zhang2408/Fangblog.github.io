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