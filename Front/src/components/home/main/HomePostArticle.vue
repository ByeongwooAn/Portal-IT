<template>
    <article id="post-area">
        <div id="post-list">
            <div v-for="post in posts" :key="post.id" class="post">
                <div class="post-image-area">
                    <img :src="post.image" alt="게시물 이미지" />
                </div>
                <div class="post-title">{{ post.title }}</div>
                <div class="post-summary">{{ post.summary }}</div>
                <div class="post-info">
                    <span class="post-author">{{ post.author }}</span>
                    <span class="post-date">{{ post.date }}</span>
                </div>
            </div>
        </div>
    </article>
</template>

<script setup>
const posts = Array.from({ length: 25 }, (_, i) => ({
    id: i + 1,
    image: `data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAT4AAACfCAMAAABX0UX9AAAAYFBMVEXa2tpWVlbd3d1RUVFLS0vU1NSqqqpKSkpUVFTh4eGPj4/Q0NBbW1vY2Ni7u7uFhYVCQkKBgYHLy8tlZWWamppgYGC1tbXn5+fBwcF6enqurq6goKA/Pz90dHRtbW2Xl5eCPCqDAAACJElEQVR4nO3a23aiMBhAYZKASRS0xcM4Mrbv/5bDsSS/toJzgWvN/npjlYusvRKBSJIAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA+O/oTTbX0kN+JV6lM72VS4/5hfjcqXnsZukxvxCfz6xHvlCXz0zkyBdr8+3XE70b8kWafGb9y09ztuSLtPl2fuLR25R8kcf5tK//+tfkEx7l07r8rfaXrp8mn/Bw9hX1+da8rdojyCc9nH2HuphyeTv9yCeJfPrm8+ZaRTnT3umST4rzFQc5D3XVzD51ZPHeFeXz1Z+bfsneGmO3LN67onyFUba66Xe4vp+7N8knhfn8OnXKXuQXYX230b8inxTmy2y7o3Ia+pXyREI+Kcjnd6bbkdr2SzW/in7kk8Z8urTdhp5Lz002X6XmmEUBySeN+fzV9BuizpT1G1n9r1FleCYhn/SVr92M+lLq4Xp5G/QjnzTm+wh+9DB51i9lZ1djP/JJQz59CiefcvsP5/p+n+OVDPmEIZ8/GhX1G+ei3Q0Hk0/q8+lL+v1va+ZasN93X5/PV+b7fMocN9zz3jUpn6svZZp+5JOGxVul7ifGnjT5bvX5iqT4WdLsl5JPavK5evZNQz6hm33ZZpLsRL5Y+5CGSe00zfmFfAGesPonT+Tj8ciRd5anS5+nV7MVS4/5lUy8ZAksPWIAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAADgOX8B6s0hYB7/yQgAAAAASUVORK5CYII=`, // 더미 이미지
    title: `게시물 제목 ${i + 1}`,
    summary: `게시물 요약 ${i + 1}`,
    date: `2025-05-0${(i % 9) + 1}`,
    author: `작성자${(i % 5) + 1}`,
}));
</script>

<style scoped>
#post-area {
    margin-top: 20px;
}

#post-list {
    display: flex;
    flex-wrap: wrap;
    gap: 27px;
    height: 100%;
    border-radius: 10px;
}

.post {
    position: relative;
    width: 235px;
    height: 276px;
    border-color: #e3e5e8;
    border-radius: 5px;
    box-shadow: 1px 1px 5px #c2c2c2;
    margin-top: 5px;
}

.post img {
    width: 100%;
    height: 140px;
    border-top-right-radius: 5px;
    border-top-left-radius: 5px;
}

.post-title {
    font-weight: bold;
}

.post-summary {
    margin-top: 3px;
    font-size: 12px;
    color: #646464;
}

.post-info {
    width: 100%;
    height: 25px;
    position: absolute;
    bottom: 0;
    border-top: 1px solid #e3e5e8;
}

.post-author {
    font-size: 12px;
}

.post-date {
    margin-top: 3px;
    margin-left: 5px;
    font-size: 12px;
    color: #646464;
}
</style>
