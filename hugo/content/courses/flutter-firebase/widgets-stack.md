---
title: Stack
description: Position widgets on a Stack
weight: 14
lastmod: 2019-07-13T10:13:30-04:00
draft: false
emoji: 🐦
vimeo: 336025721
---

## Example Code

{{< file "dart" "main.dart" >}}
{{< highlight dart >}}
class MyApp extends StatelessWidget {
 @override
 Widget build(BuildContext context) {
   return MaterialApp(
     home: Scaffold(
       body: SizedBox.expand(
         child: Stack(
           children: <Widget>[
             Icon(
               Icons.camera,
               size: 100,
               color: Colors.red,
             ),
             Align(
                 alignment: Alignment.center,
                 child: Icon(
                   Icons.camera,
                   size: 100,
                   color: Colors.blue,
                 )),
             Positioned(
                 bottom: 20,
                 left: 100,
                 child: Icon(
                   Icons.camera,
                   size: 100,
                   color: Colors.green,
                 ))
           ],
         ),
       ),
     ),
   );
 }
}
{{< /highlight >}}