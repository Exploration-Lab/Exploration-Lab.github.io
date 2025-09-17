---
layout: '../../../layouts/research-area.astro'
title: 'Machine Unlearning'
priority: 3
description: 'LLMs tend to memorize information including PI information leading to privacy issues. Machine Unlearning is a new setup wherein a pretrained model is made to "forget" certain information regarding some users who request their data to be removed.'
image: '/img/research/unlearning.png'
# image: 'https://upload.wikimedia.org/wikipedia/commons/7/7b/Robot-judge.svg'
items: [
    {
        key: 'publications',
        title: 'Publications',
        priority: 1
    },
    {
        key: 'patents',
        title: 'Patents',
        priority: 2
    },
    {
        key: 'datasets',
        title: 'Resources and Datasets',
        priority: 3
    }
]
publications: [
    {
        title: 'ReLU: Towards Robust Evaluation of Unlearning in LLMs via Data Transformations',
        authors: 'Abhinav Joshi, Shaswati Saha, Divyaksh Shukla, Sriram Vema, Harsh Jhamtani, Manas Gaur, Ashutosh Modi',
        conference: 'Findings of the Association for Computational Linguistics: EMNLP 2024',
        link: 'https://aclanthology.org/2024.findings-emnlp.706/',
        image: ''
    }
]
patents: [
    {
        title: 'Patent 1',
        authors: 'Author 1, Author 2',
        details: 'details',
        description: 'description',
        link: '#',
        image: ''
    }
]
datasets: [
    {
        title: 'ReLU: Towards Robust Evaluation of Unlearning in LLMs via Data Transformations',
        description: '',
        paper: 'ReLU: Towards Robust Evaluation of Unlearning in LLMs via Data Transformations',
        paper-link: 'https://aclanthology.org/2024.findings-emnlp.706/',
        link: 'https://exploration-lab.github.io/ReLU/',
        image: ''
    }
]
---
# Machine Unlearning

LLMs tend to memorize information including PI information leading to privacy issues. Machine Unlearning is a new setup wherein a pretrained model is made to "forget" certain information regarding some users who request their data to be removed.
