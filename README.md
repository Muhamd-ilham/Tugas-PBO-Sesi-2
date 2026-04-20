<h1 align="center">Tugas Pemrograman Berorientasi Objek - Sesi II</h1>

<p>Repository ini berisi penyelesaian Tugas Sesi II untuk mata kuliah <b>PBO</b> yang mencakup pemahaman konsep dasar Class, Object, serta perbaikan kode program Java.</p>

<hr>

<h2>📚 1. Landasan Teori</h2>

<h3>A. Definisi Class dan Object</h3>
<ul>
  <li><b>Class:</b> Sebuah <i>blueprint</i> atau kerangka dasar yang mendefinisikan atribut (data) dan metode (perilaku) yang akan dimiliki oleh objek[cite: 296].</li>
  <li><b>Object:</b> Instansiasi atau wujud nyata dari sebuah class yang memiliki status (state) dan perilaku tertentu[cite: 296].</li>
</ul>

<h3>B. Jenis-jenis Method dalam Java</h3>
<ul>
  <li><b>Method Void:</b> Method yang hanya melakukan aksi tanpa mengembalikan nilai, ditandai dengan keyword <code>void</code>[cite: 297].</li>
  <li><b>Method Non-Void (Return):</b> Method yang mengembalikan nilai dengan tipe data tertentu seperti String atau Integer[cite: 297].</li>
  <li><b>Method Static:</b> Method yang dapat dipanggil langsung melalui nama kelas tanpa harus membuat objek[cite: 297].</li>
</ul>

<hr>

<h2>💻 2. Penjelasan Kode (Komputer.java)</h2>
<p>Berdasarkan struktur kode pada file <code>Komputer.java</code>, berikut adalah bagian-bagian utamanya [cite: 300-321]:</p>
<ul>
  <li><b>Bagian 1:</b> Deklarasi nama Class yaitu <code>Komputer</code>[cite: 300].</li>
  <li><b>Bagian 2:</b> Atribut atau variabel member (<code>jenis_komputer</code> dan <code>merk</code>)[cite: 302, 304].</li>
  <li><b>Bagian 3:</b> Method Setter (<code>setDataKomputer</code>) untuk mengisi nilai ke dalam atribut[cite: 305].</li>
  <li><b>Bagian 4 & 5:</b> Method Getter untuk mengambil kembali nilai dari atribut[cite: 308, 313].</li>
  <li><b>Bagian 6:</b> Instansiasi objek baru dengan nama <code>mykom</code>[cite: 317].</li>
  <li><b>Bagian 7 & 8:</b> Proses pengisian data dan menampilkan output ke layar monitor[cite: 317, 319].</li>
</ul>

<hr>

<h2>🛠️ 3. Perbaikan Kode (HandPhone.java)</h2>
<p>Berikut adalah kode program <code>HandPhone.java</code> yang telah diperbaiki agar memenuhi standar sintaks Java sehingga dapat dikompilasi dengan benar[cite: 326]:</p>

<pre><code>
public class HandPhone {
    String jenis_hp;
    int tahun_pembuatan;

    public void setDataHP(String jenis, int tahun) {
        this.jenis_hp = jenis;
        this.tahun_pembuatan = tahun;
    }

    public String getJenisHP() {
        return jenis_hp;
    }

    public int getTahunPembuatan() {
        return tahun_pembuatan;
    }

    public static void main(String[] args) {
        HandPhone hp = new HandPhone();
        hp.setDataHP("Samsung S24", 2024);
        System.out.println("Jenis HP: " + hp.getJenisHP());
        System.out.println("Tahun: " + hp.getTahunPembuatan());
    }
}
</code></pre>

<hr>

<h2>🚀 Cara Menjalankan</h2>
<ol>
  <li>Pastikan <b>JDK</b> sudah terinstal di laptop Anda.</li>
  <li>Buka terminal atau command prompt di folder project.</li>
  <li>Kompilasi file: <code>javac HandPhone.java</code></li>
  <li>Jalankan program: <code>java HandPhone</code></li>
</ol>
