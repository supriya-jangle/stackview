import 'package:flutter/material.dart';
void main() => runApp(MyApp());
class MyApp extends StatelessWidget {
 @override
 Widget build(BuildContext context) {
 return MaterialApp(
 home: StackDemo(),
 );
 }
}
class StackDemo extends StatelessWidget {
 @override
 Widget build(BuildContext context) {
 return Scaffold(
 appBar: AppBar(title: Text('Stack Widget Example')),
 body: Center(
 child: Stack(
 alignment: Alignment.center, // Align all children to the 
center of the stack
 children: <Widget>[
 Container(
 width: 200,
 height: 200,
 color: Colors.blue,
 ),
 Positioned(
 top: 20,
 left: 20,
 child: Container(
 width: 100,
 height: 100,
 color: Colors.red,
 ),
 ),
 Positioned(
 bottom: 20,
 right: 20,
 child: Container(
 width: 50,
 height: 50,
 color: Colors.green,
 ),
 ),
 ],
 ),
 ),
 );
 }
}
