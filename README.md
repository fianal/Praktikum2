# Pertemuan 4
# Praktikum2
### Made By Alfian Nur Rizki
### NIM 312310665
### TI 23.A6

<p> Buatlah kode program java untuk:</p>

+ Mendeklarasikan class `Person`, dengan atribut `Nama`, `JenisKelamin`, `Umur` dan lengkapi dengan `access modifier`.
+ Buatlah dua buah objek dari class `Person` bernama `Anton` dan `Riko` dan panggil method `setter` dan `getter`.

<p>Tampilan Program</p>

![gambar](https://github.com/fianal/Praktikum2/blob/main/Pertemuan%204/personsetget.png)

<p>Tampilan Output</p>

![gambar](https://github.com/fianal/Praktikum2/blob/main/Pertemuan%204/Personotpsg.png)

### Source Code

```Java

class Person {
    
    private String nama;    // Atribut dengan access modifier private
    private String jenisKelamin;
    private int umur;

    
    public Person(String nama, String jenisKelamin, int umur) { // Constructor untuk menginisialisasi objek Person
        this.nama = nama;
        this.jenisKelamin = jenisKelamin;
        this.umur = umur;
    }

    
    public String getNama() {   // Getter untuk atribut Nama
        return nama;
    }

    
    public void setNama(String nama) {  // Setter untuk atribut Nama
        this.nama = nama;
    }

    
    public String getJenisKelamin() {   // Getter untuk atribut Jenis Kelamin
        return jenisKelamin;
    }

    
    public void setJenisKelamin(String jenisKelamin) {  // Setter untuk atribut Jenis Kelamin
        this.jenisKelamin = jenisKelamin;
    }

    
    public int getUmur() {  // Getter untuk atribut Umur
        return umur;
    }

   
    public void setUmur(int umur) { // Setter untuk atribut Umur
        this.umur = umur;
    }

    
    public void tampilkanInfo() {   // Method untuk menampilkan informasi Person
        System.out.println("Nama: " + nama);
        System.out.println("Jenis Kelamin: " + jenisKelamin);
        System.out.println("Umur: " + umur + " tahun");
        System.out.println();
    }

    public static void main(String[] args) {
        
        Person anton = new Person("Anton", "Laki-Laki", 21);    // Membuat objek Anton dan Riko dari class Person // 
        Person riko = new Person("Riko", "Laki-Laki", 19);

        
        anton.setNama("Anton Pratama"); // Memanggil method setter untuk mengubah data //
        anton.setUmur(25);  
        anton.setJenisKelamin("Laki-Laki");

        riko.setUmur(21); 
        riko.setNama("Riko Jaksamana");  
        riko.setJenisKelamin("Laki-Laki");

                                        
        System.out.println("Informasi Anton:");     // Menampilkan informasi Anton dan Riko
        anton.tampilkanInfo();

        System.out.println("Informasi Riko:");
        riko.tampilkanInfo();
    }
}



