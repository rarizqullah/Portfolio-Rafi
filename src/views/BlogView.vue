<template>
  <div class="container mx-auto p-3 md:p-8 flex justify-center items-center">
    <div class="flex flex-col relative w-full md:w-2/3 gap-8">
      <!-- Konten untuk Sertifikat -->
      <div
        class="certificate-section flex flex-col gap-4 md:px-20 fade-zoom-up"
      >
        <!-- Sertifikat Pertama -->
        <h1 class="text-2xl font-bold text-white">Sertifikat Penghargaan</h1>

        <!-- Deskripsi singkat -->
        <p class="text-teal-400">Coursera Google Data Analytics</p>

        <!-- Gambar sertifikat -->
        <div
          class="certificate-frame border-4 border-gray-300 shadow-lg rounded-lg overflow-hidden"
        >
          <img
            :src="certificateImage"
            alt="Sertifikat Penghargaan"
            class="certificate-image"
          />
        </div>

        <!-- Tombol aksi (Read More) -->
        <div>
          <a
            href="https://coursera.org/share/8183c5355171ad152e948ae4f23ab818"
            target="_blank"
            class="bg-teal-500 text-white px-4 py-2 rounded-md hover:bg-teal-600 transition duration-300"
          >
            Read More
          </a>
        </div>
      </div>

      <!-- Sertifikat Kedua -->
      <div
        class="certificate-section flex flex-col gap-4 md:px-20 fade-zoom-up"
      >
        <h1 class="text-2xl font-bold text-white">Sertifikat Penghargaan</h1>
        <p class="text-teal-400">Database Design and Programming with SQL</p>

        <div
          class="certificate-frame border-4 border-gray-300 shadow-lg rounded-lg overflow-hidden"
        >
          <img
            :src="certificateImageTwo"
            alt="Sertifikat Penghargaan"
            class="certificate-image"
          />
        </div>

        <div>
          <a
            href="https://coursera.org/share/another-cert-link"
            target="_blank"
            class="bg-teal-500 text-white px-4 py-2 rounded-md hover:bg-teal-600 transition duration-300"
          >
            Read More
          </a>
        </div>
      </div>

      <!-- Sertifikat Ketiga -->
      <div
        class="certificate-section flex flex-col gap-4 md:px-20 fade-zoom-up"
      >
        <h1 class="text-2xl font-bold text-white">Sertifikat Penghargaan</h1>
        <p class="text-teal-400">Database Programming with PL/SQL</p>

        <div
          class="certificate-frame border-4 border-gray-300 shadow-lg rounded-lg overflow-hidden"
        >
          <img
            :src="certificateImageTree"
            alt="Sertifikat Penghargaan"
            class="certificate-image"
          />
        </div>

        <div>
          <a
            href="https://coursera.org/share/another-cert-link"
            target="_blank"
            class="bg-teal-500 text-white px-4 py-2 rounded-md hover:bg-teal-600 transition duration-300"
          >
            Read More
          </a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      certificateImage: require("@/assets/sertifikat_coursera.png"), // Path gambar sertifikat pertama
      certificateImageTwo: require("@/assets/sertifikat_oracle1.png"), // Path gambar sertifikat kedua
      certificateImageTree: require("@/assets/sertifikat_oracle2.png"), // Path gambar sertifikat ketiga
    };
  },
};
</script>

<style scoped>
/* Styling untuk memastikan konten berada di tengah layar secara horizontal dan vertikal */
.container {
  min-height: 100vh; /* Pastikan tinggi kontainer penuh layar */
}

.certificate-frame {
  margin-top: 10px;
  width: 100%;
  height: auto;
}

.certificate-image {
  width: 100%;
  object-fit: cover;
  border-radius: 8px;
}

.certificate-section {
  background-color: #25272a; /* Tambahkan warna latar belakang */
  padding: 20px;
  border-radius: 10px;
}

/* Styling untuk tombol */
a {
  transition: background-color 0.3s ease;
}

a:hover {
  background-color: #38b2ac;
}
</style>
