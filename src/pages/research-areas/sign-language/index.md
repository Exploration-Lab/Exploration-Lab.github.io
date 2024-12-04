---
layout: '../../../layouts/research-area.astro'
title: 'Indian Sign Language Generation and Translation'
priority: 1
description: 'A small description about the things handled in Sign '
image: '/img/research/isl.jpg'
# Indian Sign Language

We are working to improve Indian Sign Language (ISL) processing by creating datasets and models that bridge the communication gap for the hard-of-hearing community. ISL, used by millions, lacks the resources needed for tasks like machine translation and recognition, leaving it behind languages such as American Sign Language. To address this, we developed CISLR, a dataset with 4700 ISL words and a model that learns from American Sign Language for better recognition; ISLTranslate, a dataset of 31,000 ISL-English sentence pairs for translation; and iSign, a benchmark with multiple tasks like video-to-text translation to aid ISL research. Our work aims to break communication barriers and promote inclusivity, with future efforts focused on expanding datasets, refining translation models, and supporting applications in areas like education and healthcare.
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
        description: 'Indian Sign Language, though used by a diverse community, still lacks well-annotated resources for developing systems that would enable sign language processing. In recent years researchers have actively worked for sign languages like American Sign Languages, however, Indian Sign language is still far from data-driven tasks like machine translation. To address this gap, in this paper, we introduce a new dataset CISLR (Corpus for Indian Sign Language Recognition) for word-level recognition in Indian Sign Language using videos. The corpus has a large vocabulary of around 4700 words covering different topics and domains. Further, we propose a baseline model for word recognition from sign language videos. To handle the low resource problem in the Indian Sign Language, the proposed model consists of a prototype-based one-shot learner that leverages resource rich American Sign Language to learn generalized features for improving predictions in Indian Sign Language. Our experiments show that gesture features learned in another sign language can help perform one-shot predictions in CISLR.',
        paper: 'CISLR: Corpus for Indian Sign Language Recognition',
        paper-link: 'https://aclanthology.org/2022.emnlp-main.707/',
        link: 'https://github.com/Exploration-Lab/CISLR',
        image: '/img/Posters/Sign-Language/CISLR.jpg'
    },
    {
        title: 'ISLTranslate: Dataset for Translating Indian Sign Language',
        description: 'Sign languages are the primary means of communication for many hard-of-hearing people worldwide. Recently, to bridge the communication gap between the hard-of-hearing community and the rest of the population, several sign language translation datasets have been proposed to enable the development of statistical sign language translation systems. However, there is a dearth of sign language resources for the Indian sign language. This resource paper introduces ISLTranslate, a translation dataset for continuous Indian Sign Language (ISL) consisting of 31k ISL-English sentence/phrase pairs. To the best of our knowledge, it is the largest translation dataset for continuous Indian Sign Language. We provide a detailed analysis of the dataset. To validate the performance of existing end-to-end Sign language to spoken language translation systems, we benchmark the created dataset with a transformer-based model for ISL translation.',
        paper: 'ISLTranslate: Dataset for Translating Indian Sign Language',
        paper-link: 'https://aclanthology.org/2023.findings-acl.665/',
        link: 'https://github.com/Exploration-Lab/ISLTranslate',
        image: '/img/Posters/Sign-Language/EtiCor.jpg'
    },
    {
        title: 'iSign: A Benchmark for Indian Sign Language Processing',
        description: 'Indian Sign Language has limited resources for developing machine learning and data-driven approaches for automated language processing. Though text/audio-based language processing techniques have shown colossal research interest and tremendous improvements in the last few years, Sign Languages still need to catch up due to the need for more resources. To bridge this gap, in this work, we propose iSign: a benchmark for Indian Sign Language (ISL) Processing. We make three primary contributions to this work. First, we release one of the largest ISL-English datasets with more than video-sentence/phrase pairs. To the best of our knowledge, it is the largest sign language dataset available for ISL. Second, we propose multiple NLP-specific tasks (including SignVideo2Text, SignPose2Text, Text2Pose, Word Prediction, and Sign Semantics) and benchmark them with the baseline models for easier access to the research community. Third, we provide detailed insights into the proposed benchmarks with a few linguistic insights into the working of ISL. We streamline the evaluation of Sign Language processing, addressing the gaps in the NLP research community for Sign Languages.',
        paper: 'iSign: A Benchmark for Indian Sign Language Processing',
        paper-link: 'https://aclanthology.org/2024.findings-acl.643/',
        link: 'https://exploration-lab.github.io/iSign/',
        image: '/img/Posters/Sign-Language/iSign.jpg'
    }
]


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
            max-width: 100%;
            height: auto;
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
        <img src="/img/Posters/Sign-Language/CISLR.jpg" alt="CISLR">
    </div>
    <div class="slide">
        <img src="/img/Posters/Sign-Language/EtiCor.jpg" alt="ISLTranslate">
    </div>
    <div class="slide">
        <img src="/img/Posters/Sign-Language/iSign.jpg" alt="iSign">
    </div>
</div>

<div class="dots">
    <span class="dot" onclick="currentSlide(1)"></span>
    <span class="dot" onclick="currentSlide(2)"></span>
    <span class="dot" onclick="currentSlide(3)"></span>
</div>
---
