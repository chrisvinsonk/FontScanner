<!-- FAQSection.vue -->
<template>
    <section class="faq-section">
        <h2>Frequently Asked Questions</h2>
        <div v-for="(item, index) in faqItems" :key="index" class="faq-item">
            <h3 class="question">{{ item.question }}</h3>
            <div class="answer">{{ item.answer }}</div>
        </div>
    </section>
</template>

<script>
export default {
    data() {
        return {
            faqItems: [
                {
                    question: "What are the symptoms of COVID-19?",
                    answer: "Common symptoms include fever, cough, and shortness of breath.",
                },
                {
                    question: "How can I protect myself from COVID-19?",
                    answer: "Practice good hand hygiene, wear masks, and maintain social distancing.",
                },
                {
                    question: "Where can I find COVID-19 testing centers?",
                    answer: "You can check with local health departments or healthcare providers.",
                },
                // Add more FAQ items as needed
            ],
        };
    },
};
</script>

<style>
.faq-section {
    margin-top: 20px;
}

.faq-item {
    margin-bottom: 20px;
}

.question {
    font-size: 18px;
    font-weight: bold;
}

.answer {
    font-size: 16px;
}
</style>
