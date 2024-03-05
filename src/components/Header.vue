<template>
    <!-- heeader start -->
    <header class="header" id="header">
        <div class="container">
            <a href="#" class="header__logo"><b>a</b>bdurohman<b>K</b>arim</a>
            <nav class="nav header__nav">
                <ul>
                    <li><a href="#home">Home</a></li>
                    <li><a href="#about">About</a></li>
                    <li><a href="#skills">Skills</a></li>
                    <li><a href="#projects">Projects</a></li>
                    <li><a href="#questions">Questions</a></li>
                </ul>
            </nav>
            <div class="actions header__actions">
                
                <button class="actions__button">EN</button>
                <button class="actions__button" id="themeToggle" @click="toggleDarkMode">
                    <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg" id="themeIcon">
                        <path opacity="0.24" d="M3 12C3 16.9706 7.02944 21 12 21C16.3981 21 20.0593 17.8386 20.8444 13.6729C20.937 13.1814 20.272 12.9415 19.9043 13.2805C18.7462 14.348 17.1992 15 15.5 15C11.9101 15 9 12.0899 9 8.5C9 6.80078 9.65202 5.25384 10.7195 4.09574C11.0585 3.72798 10.8186 3.06301 10.3271 3.15564C6.16144 3.94068 3 7.60192 3 12Z" fill="#5A6585"/>
                        <path d="M3 12C3 16.9706 7.02944 21 12 21C16.3981 21 20.0593 17.8386 20.8444 13.6729C20.937 13.1814 20.272 12.9415 19.9043 13.2805C18.7462 14.348 17.1992 15 15.5 15C11.9101 15 9 12.0899 9 8.5C9 6.80078 9.65202 5.25384 10.7195 4.09574C11.0585 3.72798 10.8186 3.06301 10.3271 3.15564C6.16144 3.94068 3 7.60192 3 12Z" stroke="#5A6585" stroke-width="2" stroke-linecap="round"/>
                    </svg>
                </button>
                <button class="actions__button" id="menuToggle" >
                    <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <g opacity="0.24">
                        <path d="M3 5C3 3.89543 3.89543 3 5 3H8C9.10457 3 10 3.89543 10 5V8C10 9.10457 9.10457 10 8 10H5C3.89543 10 3 9.10457 3 8V5Z" fill="#5A6585"/>
                        <path d="M14 5C14 3.89543 14.8954 3 16 3H19C20.1046 3 21 3.89543 21 5V8C21 9.10457 20.1046 10 19 10H16C14.8954 10 14 9.10457 14 8V5Z" fill="#5A6585"/>
                        <path d="M3 16C3 14.8954 3.89543 14 5 14H8C9.10457 14 10 14.8954 10 16V19C10 20.1046 9.10457 21 8 21H5C3.89543 21 3 20.1046 3 19V16Z" fill="#5A6585"/>
                        <path d="M14 16C14 14.8954 14.8954 14 16 14H19C20.1046 14 21 14.8954 21 16V19C21 20.1046 20.1046 21 19 21H16C14.8954 21 14 20.1046 14 19V16Z" fill="#5A6585"/>
                        </g>
                        <path d="M3 5C3 3.89543 3.89543 3 5 3H8C9.10457 3 10 3.89543 10 5V8C10 9.10457 9.10457 10 8 10H5C3.89543 10 3 9.10457 3 8V5Z" stroke="#5A6585" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                        <path d="M14 5C14 3.89543 14.8954 3 16 3H19C20.1046 3 21 3.89543 21 5V8C21 9.10457 20.1046 10 19 10H16C14.8954 10 14 9.10457 14 8V5Z" stroke="#5A6585" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                        <path d="M3 16C3 14.8954 3.89543 14 5 14H8C9.10457 14 10 14.8954 10 16V19C10 20.1046 9.10457 21 8 21H5C3.89543 21 3 20.1046 3 19V16Z" stroke="#5A6585" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                        <path d="M14 16C14 14.8954 14.8954 14 16 14H19C20.1046 14 21 14.8954 21 16V19C21 20.1046 20.1046 21 19 21H16C14.8954 21 14 20.1046 14 19V16Z" stroke="#5A6585" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                    </svg>
                </button>
            </div>
        </div>
        <nav id="navMenu">
            <ul>
                <li><a href="#home" class="navMenu__link">Home</a></li>
                <li><a href="#about" class="navMenu__link">About</a></li>
                <li><a href="#skills" class="navMenu__link">Skills</a></li>
                <li><a href="#projects" class="navMenu__link">Projects</a></li>
                <li><a href="#questions" class="navMenu__link">Questions</a></li>
            </ul>
        </nav>
    </header>
    <!-- heeader end -->
</template>
<script>
export default{
    
}
</script>
<style scoped>
    
</style>