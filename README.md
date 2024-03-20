import 'package:flutter/material.dart';
import 'package:stateless_widget1/My_page.dart';

void main() {
  runApp(MaterialApp(
    title: "Stateless widget",
    color: Colors.blue,
    theme: ThemeData(
        primarySwatch: Colors.brown,
        brightness: Brightness.dark,
        fontFamily: "Ind"),
    home: Scaffold(
      backgroundColor: Colors.black87,
      appBar: AppBar(
        title: Text('FirstScreen'),
        leading: Icon(Icons.home),
        centerTitle: true,
        backgroundColor: Colors.amber,
      ),
      body: Center(child: MyPage2()),
      floatingActionButton: FloatingActionButton(
          child: Icon(Icons.add_a_photo_rounded),
          backgroundColor: Colors.black87,
          onPressed: null),
    ),
  ));
}

class MyPage extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return Text("I am a satateless widget. I don't change never");
  }
}
import 'package:flutter/material.dart';

class MyPage2 extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return Container(
      child: Text("I am from different file"),
    );
  }
}
