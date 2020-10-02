# Console App

Aplikasi ini mencakup fungsi perhitungan nilai tukar mata uang dolar ke rupiah.
Satu dolar dianggap senilai Rp15.000

## Scope & Functionalities
* User dapat memasukkan angka
* User dapat menyentuh tombol hitung
* User mendapat info "INVALID" jika yang dimasukkan berupa teks.

## How does it works?
Diawali dari method "MainWindow" pada class MainWindow.xaml.cs kita mendeklarasikan blablabla
```c#
public MainWindow()
{
    InitializeComponent();
    currency = new CurrencyController();
}
```
Logika perhitungan terdapat pada `CurrencyController.cs`
```c#
public string usdToIdr(string nominal)
{
    var nominalDouble = Convert.ToDouble(nominal);
    var Result = nominalDouble * 15000;
    return Convert.ToString(result);
} 
```