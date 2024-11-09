<template>
    <div>
        <v-row no-gutters>
            <v-col cols="1">
                <v-img :width="30" :height="30" :src="imageSrc" alt="devops logo"></v-img>
            </v-col>
            <v-col cols="5" >
                <h2>Artificial intelligence </h2>
            </v-col>
        </v-row>
        <ul>
            <li>Having experience in using large language models models llama2/3 and phi3 via ollama.</li>

            <li>Experience in designing multi-agent workflow using langgraph </li>
            <li>Developed a RAG application for faster searching of documentation using langchain.</li>
            <li>Realtime experience in integrating openai chatgpt-4 using langchain.</li>
            <li>Having experience in vector database and embeddings.</li>
            <li>Developing an ai-interview assistant </li>
        </ul>

    </div>
</template>

<script>
import imageSrc from '@/assets/technologylogo/AI.png'

export default {
    name: 'MyComponent',
    data() {
        return {
            imageSrc
        };
    }
}
</script>