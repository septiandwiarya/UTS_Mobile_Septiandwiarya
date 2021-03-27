# UTS_Mobile_Septiandwiarya
UTS Mobile Septian Dwi Arya
import 'package:flutter/material.dart';

void main() {
  runApp(MaterialApp(
    debugShowCheckedModeBanner: false,
    title : 'Routing Navigation',
    initialRoute : '/',
    routes : {
      '/' : (context) => Menu(),
      HalamanPertama.routeName : (context) => HalamanPertama(),
      HalamanKedua.routeName : (context) => HalamanKedua(),
      HalamanKetiga.routeName : (context) => HalamanKetiga(),
      HalamanKeempat.routeName : (context) => HalamanKeempat(),
      HalamanKelima.routeName : (context) => HalamanKelima(),
      HalamanKeenam.routeName : (context) => HalamanKeenam(),
    },
  ));
}

class Menu extends StatelessWidget {
  @override
  Widget build (BuildContext context) {
    return Scaffold(
       backgroundColor : Colors.deepOrangeAccent,
      appBar : AppBar(
        backgroundColor : Colors.deepOrangeAccent,
        title : Text ('BIOGRAFI'),
      ),
      body : Center(
        child : GridView.count(
          crossAxisCount: 3,
            children:<Widget>[RaisedButton(
              child : Text ('DATA DIRI'),
              color: Colors.blueAccent,
              onPressed: (){

                Navigator.pushNamed(context, HalamanPertama.routeName);
              },
            ),
            RaisedButton(
              child : Text('INFORMASI KELUARGA'),
              color: Colors.blueAccent,
              onPressed : (){

                Navigator.pushNamed(context, HalamanKedua.routeName);
              },
            ),
            RaisedButton(
              child : Text('PRESTASI SEUMUR HIDUP'),
              color: Colors.blueAccent,
              onPressed : (){

                Navigator.pushNamed(context, HalamanKetiga.routeName);
              },
            ),
            RaisedButton(
              child : Text('JENJANG PENDIDIKAN'),
              color: Colors.blueAccent,
              onPressed : (){

                Navigator.pushNamed(context, HalamanKeempat.routeName);
              },
            ),
            RaisedButton(
              child : Text('MAKES & MIKES'),
              color: Colors.blueAccent,
              onPressed : (){

                Navigator.pushNamed(context, HalamanKelima.routeName);
              },
            ),
            RaisedButton(
              child : Text('KATA-KATA MUTIARA'),
              color: Colors.blueAccent,
              onPressed : (){

                Navigator.pushNamed(context, HalamanKeenam.routeName);
              },
            ),
          ],
        ),
      ),
    );
  }
}
class HalamanPertama extends StatelessWidget {
  static const String routeName = "/halamanPertama";
  @override
  Widget build(BuildContext context){
    return Scaffold (
      backgroundColor : Colors.lightBlueAccent,
      appBar : AppBar(
        backgroundColor : Colors.deepOrangeAccent,
        title : Text("DATA DIRI"),
      ),
      body: Center(
        child : RaisedButton(
          child : Text('Kembali'),
          onPressed:(){
            Navigator.pop(context);
          },
        ),
      ),
    );
  }
}
class HalamanKedua extends StatelessWidget {
  static const String routeName = "/halamanKedua";
  @override
  Widget build(BuildContext context){
    return Scaffold (
      backgroundColor : Colors.lightBlueAccent,
      appBar : AppBar(
        backgroundColor : Colors.deepOrangeAccent,
        title : Text("INFORMASI KELUARGA"),
      ),
      body: Center(
        child : RaisedButton(
          child : Text('Kembali'),
          onPressed:(){
            Navigator.pop(context);
          },
        ),
      ),
    );
  }
}
class HalamanKetiga extends StatelessWidget {
  static const String routeName = "/halamanKetiga";
  @override
  Widget build(BuildContext context){
    return Scaffold (
      backgroundColor : Colors.lightBlueAccent,
      appBar : AppBar(
         backgroundColor : Colors.deepOrangeAccent,
        title : Text("PRESTASI"),
      ),
      body: Center(
        child : RaisedButton(
          child : Text('Kembali'),
          onPressed:(){
            Navigator.pop(context);
          },
        ),
      ),
    );
  }
}class HalamanKeempat extends StatelessWidget {
  static const String routeName = "/halamanKeempat";
  @override
  Widget build(BuildContext context){
    return Scaffold (
      backgroundColor : Colors.lightBlueAccent,
      appBar : AppBar(
         backgroundColor : Colors.deepOrangeAccent,
        title : Text("PENDIDIKAN"),
      ),
      body: Center(
        child : RaisedButton(
          child : Text('Kembali'),
          onPressed:(){
            Navigator.pop(context);
          },
        ),
      ),
    );
  }
}class HalamanKelima extends StatelessWidget {
  static const String routeName = "/halamanKelima";
  @override
  Widget build(BuildContext context){
    return Scaffold (
      backgroundColor : Colors.lightBlueAccent,
      appBar : AppBar(
         backgroundColor : Colors.deepOrangeAccent,
        title : Text("MAKES & MIKES"),
      ),
      body: Center(
        child : RaisedButton(
          child : Text('Kembali'),
          onPressed:(){
            Navigator.pop(context);
          },
        ),
      ),
    );
  }
}
  
class  HalamanKeenam extends StatelessWidget {
  static const String routeName = "/halamanKeenam";
  @override
  Widget build(BuildContext context){
    return Scaffold(
      backgroundColor : Colors.lightBlueAccent,
      appBar : AppBar(
         backgroundColor : Colors.deepOrangeAccent,
        title : Text("KATA-KATA MUTIARA"),
      ),
      body: Center(
        child:Text('Halaman Keenam'),
      ),
    );
  }
}
