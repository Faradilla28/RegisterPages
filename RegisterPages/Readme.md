# Description RegisterPages
Bentuk pengenalan eventhandler(sinyal) dengan model registrasi + verifikasi.

## Scope & Functionalities
- user harus mengisikan nama
- user harus menambahkan alamat email
- user harus menambahkan nomor handphone
- user memilih verifikasi akan dikirimkan kemana
- user dapat menekan tombol "Daftar"

## How Does it works?
Diawali dari Method`MainWindow`  pada Class MainWindow.xaml.cs dengan cara deklarasi sebagai berikut:

```csharp
 public MainWindow()
        {
            InitializeComponent();
            controller = new MainWindowController();
            controller.SubcribeVerificationResult(this);

        }
```