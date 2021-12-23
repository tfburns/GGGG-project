# OIST Great Google Glass Giveaway proposal

This is my starter repo and proposal for my OIST Great Google Glass Giveaway entry. My goal would be to use the Google Glass wearable to make augmented math and language applications. The applications are written in order of current interest, i.e. math application would be the first project I would try. And features with dot-points are listed in the order I would try to implement those features.

## Augmented math application

In this augmented math application, I would like users to be able to:
- Given a writing surface with an equation written on it, on the user's [voice command](https://developers.google.com/glass-enterprise/guides/inputs-sensors#voice-commands) or [short camera button press](https://developers.google.com/glass-enterprise/guides/inputs-sensors#camera-button), capture any equations on the writing surface, convert it to LaTeX using OCR (for which there exist an [API](https://mathpix.com/ocr) or [two](https://developer.myscript.com/) already -- or I may choose to develop my own based on existing [open source solutions](https://github.com/falvaro/seshat), and then save it locally.
- Be able to send/upload saved equations to your e-mail/DropBox, etc.
- Given a graph (network) diagram on a writing surface, on the user's [voice command](https://developers.google.com/glass-enterprise/guides/inputs-sensors#voice-commands) or [long camera button press](https://developers.google.com/glass-enterprise/guides/inputs-sensors#camera-button), recognise the graph structure (with methods similar to [these](https://openaccess.thecvf.com/content/WACV2021/papers/Luo_ChartOCR_Data_Extraction_From_Charts_Images_via_a_Deep_Hybrid_WACV_2021_paper.pdf)) and save it both as a visual diagram and as a data object (with a list of the nodes and their edges). And again be able to send/upload these diagrams and data to e-mail/DropBox, etc.

## Shopping in a foreign language application

Since Glass [doesn't have GPS](https://developers.google.com/glass-enterprise/guides/inputs-sensors#location-services), I would like the user to be able to pin-point their location manually and/or refine it by starting with an estimated location using [IP-tracing via a Wi-Fi location](https://developers.google.com/maps/documentation/geolocation/overview), and for Glass to then search for [details of nearby stores/places on Google Maps](https://developers.google.com/maps/documentation/places/web-service/details). This information will be used to create a local savefile wherein we will save information we document via Glass. The main features of the applicatio (which will then be saved related to this location for the user to later refer to), will be:
- On the user's [voice command](https://developers.google.com/glass-enterprise/guides/inputs-sensors#voice-commands) or [short camera button press](https://developers.google.com/glass-enterprise/guides/inputs-sensors#camera-button), capture any language text in the center of the field of view of the [camera](https://developers.google.com/glass-enterprise/guides/inputs-sensors#camera) and translate it into the user's pre-defined preferred language, e.g. Japanese into English, then display it to the user.
- On the user's [voice command](https://developers.google.com/glass-enterprise/guides/inputs-sensors#voice-commands) or [long camera button press](https://developers.google.com/glass-enterprise/guides/inputs-sensors#camera-button), identify the object ([using object detection methods](https://en.wikipedia.org/wiki/Object_detection)) being held in the center of the field of view of the [camera](https://developers.google.com/glass-enterprise/guides/inputs-sensors#camera) and display the predicted identity of the object.
