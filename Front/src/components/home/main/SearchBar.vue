<template>
    <div id="border-gradient">
        <div id="search-box">
            <div id="search-group">
                <img src="@/assets/image/P.png" alt="logo-icon" />
                <form>
                    <input
                        id="search"
                        type="text"
                        placeholder="IT 관련 검색어를 입력해주세요."
                    />
                </form>
                <img src="@/assets/image/serach-icon.png" alt="search-icon" />
            </div>
        </div>
    </div>
</template>

<style scoped>
#border-gradient {
    border-radius: 30px;
    padding: 2px;
    background: linear-gradient(135deg, #0033ff 40%, #3b11f8 100%);
}

#search-box {
    background-color: white;
    width: 708px;
    height: 60px;
    border-radius: 28px;
    align-content: center;
}

#search-group {
    display: flex;
    width: 676px;
    margin: 0 auto;
    align-items: center;
}

#search {
    margin-left: 10px;
    width: 616px;
    height: 40px;
    border: none;
    outline: 1px;
    font-size: 18px;
    font-weight: bold;
}

#search::placeholder {
    color: #e3e5e8;
    font-weight: normal;
}
</style>
