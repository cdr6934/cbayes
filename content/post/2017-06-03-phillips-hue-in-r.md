---
title: 'Phillips Hue in R '
author: Chris Ried
date: '2017-06-03'
slug: phillips-hue-in-r
categories:
  - R
tags:
  - iot
  - R
---


```
getIP <- function()
{
  url <- paste0("https://www.meethue.com/api/nupnp")
  res <- httpGET(url)
  resJson <- fromJSON(res)
  res <- resJson[["internalipaddress"]]
  res
}



#Finding the bridge 
# TODO: https://huetips.com/help/how-to-find-my-bridge-ip-address/

#############################################################
# Get the light 
#############################################################
getLights <- function(ip, userName) 
{ 
  ip <- getIP()
  url <- paste0("http://",ip,"/api/",userName,"/lights/")
  #content <- paste0('{"on":',state,'}')
  res <- httpGET(url)
  res
}
getLights(ip, userName)
```
