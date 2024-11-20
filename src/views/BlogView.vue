<template>

<header>
        <div
          class="text-2xl font-bold text-white mb-10 md:py-10 fadein-bot title-section flex items-center justify-center flex-col"
        >
          <h4>certificate of appreciation</h4>
          <h4
            class="text-base font-normal text-transparent bg-clip-text bg-gradient-to-r from-slate-100 to-gray-500"
          >
          Successes I've Achieved So Far
          </h4>
        </div>
      </header>

  <div class="container mx-auto p-3 md:p-1 flex justify-center items-center fade-in">
    <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
      <!-- Sertifikat Pertama -->
      <div class="certificate-card bg-black text-white rounded-lg shadow-lg overflow-hidden">
        <div class="card-header p-4">
          <p class="text-gray-400  text-sm">Coursera Google Data Analytics</p>
        </div>
        <div class="card-image">
          <img
            :src="certificateImage"
            alt="Sertifikat Penghargaan"
            class="object-contain w-full h-40"
          />
        </div>
        <div class="card-footer p-4">
          <a
            href="https://coursera.org/share/8183c5355171ad152e948ae4f23ab818"
            target="_blank"
            class="bg-gray-800 text-white px-3 py-2 text-sm rounded-md hover:bg-teal-600 transition"
          >
            Read More
          </a>
        </div>
      </div>

      <!-- Sertifikat Kedua -->
      <div class="certificate-card bg-black text-white rounded-lg shadow-lg overflow-hidden">
        <div class="card-header p-4">
          <p class="text-gray-400 text-sm">Database Design and Programming with SQL</p>
        </div>
        <div class="card-image">
          <img
            :src="certificateImageTwo"
            alt="Sertifikat Penghargaan"
            class="object-contain w-full h-40"
          />
        </div>
        <div class="card-footer p-4">
          <a
            href="https://drive.google.com/file/d/1kU5LW6XCMHwz86MQ82vZEjcqsTti2zBH/view?usp=sharing"
            target="_blank"
            class="bg-gray-800 text-white px-3 py-2 text-sm rounded-md hover:bg-teal-600 transition"
          >
            Read More
          </a>
        </div>
      </div>

      <!-- Sertifikat Ketiga -->
      <div class="certificate-card bg-black text-white rounded-lg shadow-lg overflow-hidden">
        <div class="card-header p-4">
          <p class="text-gray-400 text-sm">Database Programming with PL/SQL</p>
        </div>
        <div class="card-image">
          <img
            :src="certificateImageTree"
            alt="Sertifikat Penghargaan"
            class="object-contain w-full h-40"
          />
        </div>
        <div class="card-footer p-4">
          <a
            href="https://drive.google.com/file/d/1ML6K5sZzuSI_HU0elZ60-04i61sDSZ4y/view?usp=sharing"
            target="_blank"
            class="bg-gray-800 text-white px-3 py-2 text-sm rounded-md hover:bg-teal-600 transition"
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
      certificateImage: require("@/assets/sertifikat_coursera.png"),
      certificateImageTwo: require("@/assets/sertifikat_oracle1.png"),
      certificateImageTree: require("@/assets/sertifikat_oracle2.png"),
    };
  },
};
</script>

<style scoped>
.container {
  margin-top: 80px; /* Adjust to fit the height of your navbar */
}

.fade-in {
  animation: fadeIn 1s ease-in-out;
}

@keyframes fadeIn {
  from {
    opacity: 0;
    transform: translateY(10px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

.certificate-card {
  display: flex;
  flex-direction: column;
}

.card-header {
  background-color: #000000;
}

.card-image img {
  object-fit: contain;
  border-radius: 0;
}

.card-footer {
  text-align: center;
}
</style>
