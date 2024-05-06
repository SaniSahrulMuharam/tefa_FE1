
import type nuxtConfig from '~/nuxt.config';

<template>
  <div class="container-fluid">
    <div class="row">
      <div class="col-lg-12">
        <h2 class="text-center my-4">ISI BUKU KUNJUNGAN</h2>
        <form>
          <div class="mb-3">
            <input type="text" class="form-control form-control-lg rounded-3" placeholder="NAMA.....">
          </div>
          <div class="mb-3">
            <select class="form-control form-control-lg form-select rounded-3">
              <option value="">Keanggotaan</option>
              <option value="Siswa">Siswa</option>
              <option value="Guru">Guru</option>
              <option value="Stap">Stap</option>
              <option value="Umum">Umum</option>
            </select>
          </div>
          <div class="mb-3">
            <div class="row">
              <div class="col-md-4">
                <select class="form-control form-control-lg form-select rounded-3 mb-2">
                  <option value="">TINGKAT</option>
                  <option value="X">X</option>
                  <option value="XI">XI</option>
                  <option value="XII">XII</option>
                </select>
              </div>
              <div class="col-md-4">
                <select class="form-control form-control-lg form-select rounded-3 mb-2">
                  <option value="">JURUSAN</option>
                  <option value="pplg">pplg</option>
                  <option value="tjkt">tjkt</option>
                  <option value="tsm">tsm</option>
                  <option value="dkv">dkv</option>
                  <option value="toi">toi</option>
                  
                </select>
              </div>
              <div class="col-md-4">
                <select class="form-control form-control-lg form-select rounded-3 mb-2">
                  <option value="">KELAS</option>
                  <option value="1">1</option>
                  <option value="2">2</option>
                  <option value="3">3</option>
                  <option value="4">4</option>
                </select>
                </div>
              </div>
            </div>
            <div class="col-mb-3">
                <select class="form-control form-control-lg form-select rounded-3 mb-4">
                  <option value="">KEPERLUAN</option>
                  <option value="baca">baca buku</option>
                  <option value="pinjam">pinjam buku</option>
                  <option value="kembalikan">kembalikan buku</option>
                </select>
          </div>
        </form>
        <nuxt-link to="/pengunjung/">
          <button type="submit" class="btn btn-dark btn-lg rounded-3 px-5">Kirim</button>
        </nuxt-link>
      </div>
    </div>
  </div>
</template>

<style scoped>
.form-control{
  background-color: #EDEDED;
}
</style>
<!-- <script setup>
const supabase = useSupabaseClient()

const members = ref([])
const objectives = ref([])

const form = ref({
  nama: "",
  keanggotaan: "",
  tingkat: "",
  jurusan: "",
  kelas: "",
  keperluan: "",
})

const kirimData = async () => {
  const { error } = await supabase.from('pengunjung').insert([form.value])
  if(!error)navigeteTo('/pengunjung')
}

const getKeanggotaan = async () => {
  const {data,error} = await supabase.from('keanggotaan').select('*')
  if(data)members.value = data
}

const getKeperluan = async () => {
  const {data,error} = await supabase.from('keperluan').select('*')
  if(data)objectives.value = data
}

onMounted(() => {
  getkeanggotaan()
  getkeperluan()
})
</script> -->