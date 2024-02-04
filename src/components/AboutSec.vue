<template>
    <section id="about" class="w-full justify-center items-center">
        <div class="bg-white w-full min-h-screen">
            <h5 class="text-center py-6 text-xl lg:text-2xl font-medium">About Me</h5>
            <div class="flex flex-col lg:flex-row justify-center gap-8 px-6 lg:px-32">
                <aside class="font-medium w-full lg:w-1/2">
                    <h5 class="font-medium text-black border-b-2 border-black pb-1">Profile</h5>
                    <ul class="font-light text-slate-600 text-sm mt-3">
                        <li>Image:
                            <img src="../assets/erlang.png" alt="erlang.png" class="w-32 bg-blue-500 rounded-full my-3">
                        </li>
                        <li>Fullname: Erlang Andriyanputra</li>
                        <li>Birthday: Banjarmasin, 05-September-2007</li>
                        <li>Status: Student</li>
                        <li>Current School: SMKN 02 Banjarmasin</li>
                        <li>Message:
                            <p class="text-black font-normal">Hi, my name is Erlang Andriyanputra, you can call me Erlang, I'm a student at SMKN 2 Banjarmasin majoring in Software and Game Development</p>
                        </li>
                    </ul>
                </aside>
                <aside class="w-full lg:w-1/2">
                    <h5 class="font-medium text-black border-b-2 border-black pb-1">Educations</h5>
                    <ul class="font-light text-slate-600 text-sm mt-3">
                        <h5 class="font-normal">School:</h5>
                        <li v-for="s in school">{{ s.school }}: {{ s.period }}</li>
                    </ul>
                    <ul class="font-light text-slate-600 text-sm mt-3 flex flex-col gap-2">
                        <h5 class="font-normal">Certificate From School & Online Class:</h5>
                        <li v-for="certif in certificates">
                            {{ certif.title }}: {{ certif.time }}
                            <img :src="certif.image" :alt="certif.title" width="150">
                        </li>
                    </ul>
                </aside>
            </div>
        </div>
    </section>
</template>

<script setup>
    import RevouFundamental from '../assets/revou-1.jpg'
    import DigitalizFE from '../assets/digitaliz-1.jpg'

    const school = [
        {
            school: 'TK Al-Hijrah',
            period: '2012-2013'
        },
        {
            school: 'SDN Sungai Jingah 06 Banjarmasin',
            period: '2013-2019'
        },
        {
            school: 'SMPN 27 Banjarmasin',
            period: '2019-2022'
        },
        {
            school: 'SMKN 02 Banjarmasin',
            period: '2022-Current'
        },
    ]

    const certificates = [
        {
            title: 'Revou Fundamental Course',
            time: 2023,
            image: RevouFundamental
        },
        {
            title: 'Digitaliz Frontend Web Developer',
            time: 2023,
            image: DigitalizFE
        },
    ]
</script>