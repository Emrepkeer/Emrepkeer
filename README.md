```cpp
public Form1()
{
    InitializeComponent();
}

private void button1_Click(object sender, EventArgs e)
{
    double sayi1 = Convert.ToDouble(textBox1.Text);
    double sayi2 = Convert.ToDouble(textBox2.Text);

    if (radioButton1.Checked)
    {
        TekOrtalamalar ortalama = new TekOrtalamalar();
        label4.Text = ortalama.TekOrt(sayi1, sayi2).ToString();
    }
    else if (radioButton2.Checked)
    {
        ÇiftOrtalamalar ort = new ÇiftOrtalamalar();
        label4.Text = ort.ÇiftOrt(sayi1, sayi2).ToString();
    }
}





public double TekOrt(double a, double b)
{
    double toplam = 0;
    double SayiDeğeri = 0;
    double Ortalama = 0;

    if (a > b)
    {
        for (double i = b; i <= a; i++)
        {
            if (i % 2 == 1)
            {
                SayiDeğeri++;
                toplam = toplam + i;
            }
        }
        Ortalama = toplam / SayiDeğeri;
    }
    else
    {
        for (double i = a; i <= b; i++)
        {
            if (i % 2 == 1)
            {
                SayiDeğeri++;
                toplam = toplam + i;
            }
        }
        Ortalama = toplam / SayiDeğeri;
    }

    return Ortalama;
}
```
