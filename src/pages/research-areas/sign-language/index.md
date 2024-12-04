---
layout: '../../../layouts/research-area.astro'
title: 'Indian Sign Language Generation and Translation'
priority: 1
description: 'When words are out of reach, the hands sing—sign language is the art of giving silence its voice.'
image: '/img/research/isl.jpg'
items: [
    {
        key: 'publications',
        title: 'Publications',
        priority: 1
    },
    {
        key: 'datasets',
        title: 'Resources and Datasets',
        priority: 2
    }
]
publications: [
    {
        title: 'CISLR: Corpus for Indian Sign Language Recognition',
        authors: 'Abhinav Joshi , Ashwani Bhat , Pradeep S , Priya Gole , Shreyansh Agarwal , Shashwat Gupta , Ashutosh Modi',
        conference: 'Proceedings of the 2022 Conference on Empirical Methods in Natural Language Processing',
        link: 'https://aclanthology.org/2022.emnlp-main.707/',
        image: '/img/Posters/Sign-Language/CISLR.jpg'
    },
    {
        title: 'ISLTranslate: Dataset for Translating Indian Sign Language',
        authors: 'Abhinav Joshi,  Susmit Agrawal, Ashutosh Modi',
        conference: 'Findings of the Association for Computational Linguistics: ACL 2023',
        link: 'https://aclanthology.org/2023.findings-acl.665/',
        image: '/img/Posters/Sign-Language/EtiCor.jpg'
    },
    {
        title: 'iSign: A Benchmark for Indian Sign Language Processing',
        authors: 'Abhinav Joshi, Romit Mohanty, Mounika Kanakanti, Andesha Mangla, Sudeep Choudhary, Monali Barbate ,Ashutosh Modi',
        conference: 'Findings of the Association for Computational Linguistics: ACL 2024',
        link: 'https://aclanthology.org/2024.findings-acl.643/',
        image: '/img/Posters/Sign-Language/iSign.jpg'
    }
]
datasets: [
    {
        title: 'CISLR: Corpus for Indian Sign Language Recognition',
        description: '#',
        paper-link: 'https://aclanthology.org/2022.emnlp-main.707/',
        link: 'https://github.com/Exploration-Lab/CISLR',
        image: '/img/Posters/Sign-Language/CISLR.jpg'
    },
    {
        title: 'ISLTranslate: Dataset for Translating Indian Sign Language',
        description: '#',
        paper: 'ISLTranslate: Dataset for Translating Indian Sign Language',
        paper-link: 'https://aclanthology.org/2023.findings-acl.665/',
        link: 'https://github.com/Exploration-Lab/ISLTranslate',
        image: '/img/Posters/Sign-Language/EtiCor.jpg'
    },
    {
        title: 'iSign: A Benchmark for Indian Sign Language Processing',
        description: '#',
        paper: 'iSign: A Benchmark for Indian Sign Language Processing',
        paper-link: 'https://aclanthology.org/2024.findings-acl.643/',
        link: 'https://exploration-lab.github.io/iSign/',
        image: '/img/Posters/Sign-Language/iSign.jpg'
    }
]
---

# Indian Sign Language

We are working to improve Indian Sign Language (ISL) processing by creating datasets and models that bridge the communication gap for the hard-of-hearing community. ISL, used by millions, lacks the resources needed for tasks like machine translation and recognition, leaving it behind languages such as American Sign Language. To address this, we developed CISLR, a dataset with 4700 ISL words and a model that learns from American Sign Language for better recognition; ISLTranslate, a dataset of 31,000 ISL-English sentence pairs for translation; and iSign, a benchmark with multiple tasks like video-to-text translation to aid ISL research. Our work aims to break communication barriers and promote inclusivity, with future efforts focused on expanding datasets, refining translation models, and supporting applications in areas like education and healthcare.

<style>
    /* General styling for slideshow */
    .slideshow-container {
        position: relative;
        max-width: 90%;
        margin: 2rem auto;
        text-align: center;
    }

    .slide {
        display: none;
        animation: fade 1.5s ease-in-out;
    }

    .slide img {
        width: auto; /* Set this to 'auto' if you want to maintain aspect ratio */
        max-width: 400px; /* Adjust this to reduce the maximum width */
        height: 500px; /* Set a specific height if needed; adjust to your preference */
        margin: 0 auto;
    }

    .dots {
        text-align: center;
        margin-top: 15px;
    }

    .dot {
        cursor: pointer;
        height: 12px;
        width: 12px;
        margin: 5px;
        background-color: #bbb;
        border-radius: 50%;
        display: inline-block;
    }

    .dot.active {
        background-color: #717171;
    }

    @keyframes fade {
        from {
            opacity: 0.4;
        }
        to {
            opacity: 1;
        }
    }
</style>

<script>
    let currentIndex = 0;

    function showSlides() {
        const slides = document.getElementsByClassName("slide");
        const dots = document.getElementsByClassName("dot");
        for (let i = 0; i < slides.length; i++) {
            slides[i].style.display = "none";
        }
        currentIndex++;
        if (currentIndex > slides.length) currentIndex = 1;
        for (let i = 0; i < dots.length; i++) {
            dots[i].className = dots[i].className.replace(" active", "");
        }
        slides[currentIndex - 1].style.display = "block";
        dots[currentIndex - 1].className += " active";
        setTimeout(showSlides, 3000);
    }

    document.addEventListener("DOMContentLoaded", showSlides);
</script>

<!-- Slideshow -->
<div class="slideshow-container">
    <div class="slide">
        <img src="/img/Posters/Sign-Language/CISLR.jpg" alt="CISLR" loading="lazy">
    </div>
    <div class="slide">
        <img src="/img/Posters/Sign-Language/EtiCor.jpg" alt="ISLTranslate" loading="lazy">
    </div>
    <div class="slide">
        <img src="/img/Posters/Sign-Language/iSign.jpg" alt="iSign" loading="lazy">
    </div>
</div>

<div class="dots">
    <span class="dot" onclick="currentSlide(1)"></span>
    <span class="dot" onclick="currentSlide(2)"></span>
    <span class="dot" onclick="currentSlide(3)"></span>
</div>
