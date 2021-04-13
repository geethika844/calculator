# calculator
calculator app

GEETHIKA MADHURI <geethika.sree910@gmail.com>
5:58 PM (1 hour ago)
to me

{\rtf1\ansi\ansicpg1252\deff0\nouicompat\deflang1033{\fonttbl{\f0\fnil\fcharset0 Calibri;}}
{\*\generator Riched20 10.0.19041}\viewkind4\uc1 
\pard\sa200\sl276\slmult1\f0\fs22\lang9 package com.crunchify.tutorials.crunchifycalculator;\par
 \par
import android.os.Bundle;\par
import android.support.v7.app.AppCompatActivity;\par
import android.view.View;\par
import android.widget.Button;\par
import android.widget.EditText;\par
 \par
public class MainActivity extends AppCompatActivity \{\par
 \par
    Button button0, button1, button2, button3, button4, button5, button6,\par
            button7, button8, button9, buttonAdd, buttonSub, buttonDivision,\par
            buttonMul, button10, buttonC, buttonEqual;\par
    EditText crunchifyEditText;\par
 \par
    float mValueOne, mValueTwo;\par
 \par
    boolean crunchifyAddition, mSubtract, crunchifyMultiplication, crunchifyDivision;\par
 \par
    @Override\par
    protected void onCreate(Bundle savedInstanceState) \{\par
        super.onCreate(savedInstanceState);\par
        setContentView(R.layout.activity_main);\par
 \par
        button0 = (Button) findViewById(R.id.button0);\par
        button1 = (Button) findViewById(R.id.button1);\par
        button2 = (Button) findViewById(R.id.button2);\par
        button3 = (Button) findViewById(R.id.button3);\par
        button4 = (Button) findViewById(R.id.button4);\par
        button5 = (Button) findViewById(R.id.button5);\par
        button6 = (Button) findViewById(R.id.button6);\par
        button7 = (Button) findViewById(R.id.button7);\par
        button8 = (Button) findViewById(R.id.button8);\par
        button9 = (Button) findViewById(R.id.button9);\par
        button10 = (Button) findViewById(R.id.button10);\par
        buttonAdd = (Button) findViewById(R.id.buttonadd);\par
        buttonSub = (Button) findViewById(R.id.buttonsub);\par
        buttonMul = (Button) findViewById(R.id.buttonmul);\par
        buttonDivision = (Button) findViewById(R.id.buttondiv);\par
        buttonC = (Button) findViewById(R.id.buttonC);\par
        buttonEqual = (Button) findViewById(R.id.buttoneql);\par
        crunchifyEditText = (EditText) findViewById(R.id.edt1);\par
 \par
 \par
        button1.setOnClickListener(new View.OnClickListener() \{\par
            @Override\par
            public void onClick(View v) \{\par
                crunchifyEditText.setText(crunchifyEditText.getText() + "1");\par
            \}\par
        \});\par
 \par
        button2.setOnClickListener(new View.OnClickListener() \{\par
            @Override\par
            public void onClick(View v) \{\par
                crunchifyEditText.setText(crunchifyEditText.getText() + "2");\par
            \}\par
        \});\par
 \par
        button3.setOnClickListener(new View.OnClickListener() \{\par
            @Override\par
            public void onClick(View v) \{\par
                crunchifyEditText.setText(crunchifyEditText.getText() + "3");\par
            \}\par
        \});\par
 \par
        button4.setOnClickListener(new View.OnClickListener() \{\par
            @Override\par
            public void onClick(View v) \{\par
                crunchifyEditText.setText(crunchifyEditText.getText() + "4");\par
            \}\par
        \});\par
 \par
        button5.setOnClickListener(new View.OnClickListener() \{\par
            @Override\par
            public void onClick(View v) \{\par
                crunchifyEditText.setText(crunchifyEditText.getText() + "5");\par
            \}\par
        \});\par
 \par
        button6.setOnClickListener(new View.OnClickListener() \{\par
            @Override\par
            public void onClick(View v) \{\par
                crunchifyEditText.setText(crunchifyEditText.getText() + "6");\par
            \}\par
        \});\par
 \par
        button7.setOnClickListener(new View.OnClickListener() \{\par
            @Override\par
            public void onClick(View v) \{\par
                crunchifyEditText.setText(crunchifyEditText.getText() + "7");\par
            \}\par
        \});\par
 \par
        button8.setOnClickListener(new View.OnClickListener() \{\par
            @Override\par
            public void onClick(View v) \{\par
                crunchifyEditText.setText(crunchifyEditText.getText() + "8");\par
            \}\par
        \});\par
 \par
        button9.setOnClickListener(new View.OnClickListener() \{\par
            @Override\par
            public void onClick(View v) \{\par
                crunchifyEditText.setText(crunchifyEditText.getText() + "9");\par
            \}\par
        \});\par
 \par
        button0.setOnClickListener(new View.OnClickListener() \{\par
            @Override\par
            public void onClick(View v) \{\par
                crunchifyEditText.setText(crunchifyEditText.getText() + "0");\par
            \}\par
        \});\par
 \par
        buttonAdd.setOnClickListener(new View.OnClickListener() \{\par
            @Override\par
            public void onClick(View v) \{\par
 \par
                if (crunchifyEditText == null) \{\par
                    crunchifyEditText.setText("");\par
                \} else \{\par
                    mValueOne = Float.parseFloat(crunchifyEditText.getText() + "");\par
                    crunchifyAddition = true;\par
                    crunchifyEditText.setText(null);\par
                \}\par
            \}\par
        \});\par
 \par
        buttonSub.setOnClickListener(new View.OnClickListener() \{\par
            @Override\par
            public void onClick(View v) \{\par
                mValueOne = Float.parseFloat(crunchifyEditText.getText() + "");\par
                mSubtract = true;\par
                crunchifyEditText.setText(null);\par
            \}\par
        \});\par
 \par
        buttonMul.setOnClickListener(new View.OnClickListener() \{\par
            @Override\par
            public void onClick(View v) \{\par
                mValueOne = Float.parseFloat(crunchifyEditText.getText() + "");\par
                crunchifyMultiplication = true;\par
                crunchifyEditText.setText(null);\par
            \}\par
        \});\par
 \par
        buttonDivision.setOnClickListener(new View.OnClickListener() \{\par
            @Override\par
            public void onClick(View v) \{\par
                mValueOne = Float.parseFloat(crunchifyEditText.getText() + "");\par
                crunchifyDivision = true;\par
                crunchifyEditText.setText(null);\par
            \}\par
        \});\par
 \par
        buttonEqual.setOnClickListener(new View.OnClickListener() \{\par
            @Override\par
            public void onClick(View v) \{\par
                mValueTwo = Float.parseFloat(crunchifyEditText.getText() + "");\par
 \par
                if (crunchifyAddition == true) \{\par
                    crunchifyEditText.setText(mValueOne + mValueTwo + "");\par
                    crunchifyAddition = false;\par
                \}\par
 \par
                if (mSubtract == true) \{\par
                    crunchifyEditText.setText(mValueOne - mValueTwo + "");\par
                    mSubtract = false;\par
                \}\par
 \par
                if (crunchifyMultiplication == true) \{\par
                    crunchifyEditText.setText(mValueOne * mValueTwo + "");\par
                    crunchifyMultiplication = false;\par
                \}\par
 \par
                if (crunchifyDivision == true) \{\par
                    crunchifyEditText.setText(mValueOne / mValueTwo + "");\par
                    crunchifyDivision = false;\par
                \}\par
            \}\par
        \});\par
 \par
        buttonC.setOnClickListener(new View.OnClickListener() \{\par
            @Override\par
            public void onClick(View v) \{\par
                crunchifyEditText.setText("");\par
            \}\par
        \});\par
 \par
        button10.setOnClickListener(new View.OnClickListener() \{\par
            @Override\par
            public void onClick(View v) \{\par
                crunchifyEditText.setText(crunchifyEditText.getText() + ".");\par
            \}\par
        \});\par
    \}\par
\}\par
if (crunchifyAddition == true) \{\par
      crunchifyEditText.setText(mValueOne + mValueTwo + "");\par
      crunchifyAddition = false;\par
\}\par
<?xml version="1.0" encoding="utf-8"?>\par
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"\par
    xmlns:tools="http://schemas.android.com/tools"\par
    android:id="@+id/relative1"\par
    android:layout_width="match_parent"\par
    android:layout_height="match_parent"\par
    tools:context=".MainActivity">\par
 \par
    <EditText\par
        android:id="@+id/edt1"\par
        android:layout_width="match_parent"\par
        android:layout_height="wrap_content" />\par
 \par
 \par
    <Button\par
        android:id="@+id/button1"\par
        style="?android:attr/buttonStyleSmall"\par
        android:layout_width="wrap_content"\par
        android:layout_height="wrap_content"\par
        android:layout_alignEnd="@+id/button4"\par
        android:layout_alignRight="@+id/button4"\par
        android:layout_below="@+id/edt1"\par
        android:layout_marginTop="94dp"\par
        android:text="1" />\par
 \par
    <Button\par
        android:id="@+id/button2"\par
        style="?android:attr/buttonStyleSmall"\par
        android:layout_width="wrap_content"\par
        android:layout_height="wrap_content"\par
        android:layout_alignTop="@+id/button1"\par
        android:layout_toLeftOf="@+id/button3"\par
        android:layout_toStartOf="@+id/button3"\par
        android:text="2" />\par
 \par
    <Button\par
        android:id="@+id/button3"\par
        style="?android:attr/buttonStyleSmall"\par
        android:layout_width="wrap_content"\par
        android:layout_height="wrap_content"\par
        android:layout_alignTop="@+id/button2"\par
        android:layout_centerHorizontal="true"\par
        android:text="3" />\par
 \par
    <Button\par
        android:id="@+id/button4"\par
        style="?android:attr/buttonStyleSmall"\par
        android:layout_width="wrap_content"\par
        android:layout_height="wrap_content"\par
        android:layout_below="@+id/button1"\par
        android:layout_toLeftOf="@+id/button2"\par
        android:text="4" />\par
 \par
    <Button\par
        android:id="@+id/button5"\par
        style="?android:attr/buttonStyleSmall"\par
        android:layout_width="wrap_content"\par
        android:layout_height="wrap_content"\par
        android:layout_alignBottom="@+id/button4"\par
        android:layout_alignLeft="@+id/button2"\par
        android:layout_alignStart="@+id/button2"\par
        android:text="5" />\par
 \par
    <Button\par
        android:id="@+id/button6"\par
        style="?android:attr/buttonStyleSmall"\par
        android:layout_width="wrap_content"\par
        android:layout_height="wrap_content"\par
        android:layout_alignLeft="@+id/button3"\par
        android:layout_alignStart="@+id/button3"\par
        android:layout_below="@+id/button3"\par
        android:text="6" />\par
 \par
    <Button\par
        android:id="@+id/button7"\par
        style="?android:attr/buttonStyleSmall"\par
        android:layout_width="wrap_content"\par
        android:layout_height="wrap_content"\par
        android:layout_below="@+id/button4"\par
        android:layout_toLeftOf="@+id/button2"\par
        android:text="7" />\par
 \par
    <Button\par
        android:id="@+id/button8"\par
        style="?android:attr/buttonStyleSmall"\par
        android:layout_width="wrap_content"\par
        android:layout_height="wrap_content"\par
        android:layout_alignLeft="@+id/button5"\par
        android:layout_alignStart="@+id/button5"\par
        android:layout_below="@+id/button5"\par
        android:text="8" />\par
 \par
    <Button\par
        android:id="@+id/button9"\par
        style="?android:attr/buttonStyleSmall"\par
        android:layout_width="wrap_content"\par
        android:layout_height="wrap_content"\par
        android:layout_alignLeft="@+id/button6"\par
        android:layout_alignStart="@+id/button6"\par
        android:layout_below="@+id/button6"\par
        android:text="9" />\par
 \par
    <Button\par
        android:id="@+id/buttonadd"\par
        style="?android:attr/buttonStyleSmall"\par
        android:layout_width="wrap_content"\par
        android:layout_height="wrap_content"\par
        android:layout_alignEnd="@+id/edt1"\par
        android:layout_alignRight="@+id/edt1"\par
        android:layout_alignTop="@+id/button3"\par
        android:layout_marginLeft="46dp"\par
        android:layout_marginStart="46dp"\par
        android:layout_toRightOf="@+id/button3"\par
        android:text="+" />\par
 \par
    <Button\par
        android:id="@+id/buttonsub"\par
        style="?android:attr/buttonStyleSmall"\par
        android:layout_width="wrap_content"\par
        android:layout_height="wrap_content"\par
        android:layout_alignEnd="@+id/buttonadd"\par
        android:layout_alignLeft="@+id/buttonadd"\par
        android:layout_alignRight="@+id/buttonadd"\par
        android:layout_alignStart="@+id/buttonadd"\par
        android:layout_below="@+id/buttonadd"\par
        android:text="-" />\par
 \par
    <Button\par
        android:id="@+id/buttonmul"\par
        style="?android:attr/buttonStyleSmall"\par
        android:layout_width="wrap_content"\par
        android:layout_height="wrap_content"\par
        android:layout_alignLeft="@+id/buttonsub"\par
        android:layout_alignParentEnd="true"\par
        android:layout_alignParentRight="true"\par
        android:layout_alignStart="@+id/buttonsub"\par
        android:layout_below="@+id/buttonsub"\par
        android:text="*" />\par
 \par
    <Button\par
        android:id="@+id/button10"\par
        style="?android:attr/buttonStyleSmall"\par
        android:layout_width="wrap_content"\par
        android:layout_height="wrap_content"\par
        android:layout_below="@+id/button7"\par
        android:layout_toLeftOf="@+id/button2"\par
        android:text="." />\par
 \par
    <Button\par
        android:id="@+id/button0"\par
        style="?android:attr/buttonStyleSmall"\par
        android:layout_width="wrap_content"\par
        android:layout_height="wrap_content"\par
        android:layout_alignLeft="@+id/button8"\par
        android:layout_alignStart="@+id/button8"\par
        android:layout_below="@+id/button8"\par
        android:text="0" />\par
 \par
    <Button\par
        android:id="@+id/buttonC"\par
        style="?android:attr/buttonStyleSmall"\par
        android:layout_width="wrap_content"\par
        android:layout_height="wrap_content"\par
        android:layout_alignLeft="@+id/button9"\par
        android:layout_alignStart="@+id/button9"\par
        android:layout_below="@+id/button9"\par
        android:text="C" />\par
 \par
    <Button\par
        android:id="@+id/buttondiv"\par
        style="?android:attr/buttonStyleSmall"\par
        android:layout_width="wrap_content"\par
        android:layout_height="wrap_content"\par
        android:layout_alignEnd="@+id/buttonmul"\par
        android:layout_alignLeft="@+id/buttonmul"\par
        android:layout_alignRight="@+id/buttonmul"\par
        android:layout_alignStart="@+id/buttonmul"\par
        android:layout_below="@+id/buttonmul"\par
        android:text="/" />\par
 \par
    <Button\par
        android:id="@+id/buttoneql"\par
        android:layout_width="wrap_content"\par
        android:layout_height="wrap_content"\par
        android:layout_alignEnd="@+id/buttondiv"\par
        android:layout_alignLeft="@+id/button10"\par
        android:layout_alignRight="@+id/buttondiv"\par
        android:layout_alignStart="@+id/button10"\par
        android:layout_below="@+id/button0"\par
        android:layout_marginTop="37dp"\par
        android:text="=" />\par
 \par
</RelativeLayout>\par
}

