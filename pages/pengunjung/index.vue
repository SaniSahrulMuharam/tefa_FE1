<template>
  <div class="container-fluid">
    <div class="row">
      <div class="col-lg-12">
        <h2 class="text-center my-4">RIWAYAT KUNJUNGAN</h2>
        <div class="my-3">
          <input type="search" class="form-control form-control-lg rounded-3" placeholder="filter....">
        </div>
        <div class="my-3 text-muted">menampilkan 3 dari 3</div>
        <table class="table">
          <thead>
            <tr>
              <td>#</td>
              <td>Nama</td>
              <td>Keanggotaan</td>
              <td>Waktu</td>
              <td>Keperluan</td>
            </tr>
            </thead>
            <tbody>
                <tr>
                <td>1.</td>
                <td>Sani</td>
                <td>Siswa</td>
                <td>26 Februari 2024, 12.50.00</td>
                <td>baca</td>
              </tr>
            </tbody>
        </table>
        <nuxt-link to="/">
          <button type="submit" class="btn btn-dark rounded-3 px-5">Kembali</button>
        </nuxt-link>
      </div>
    </div>
  </div>
</template>