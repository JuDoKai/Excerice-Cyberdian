<template>
    <div class="Header">
        <div class="UpperHeader">
            <nav>
                <ul>
                    <li><i class="fa-solid fa-bars"></i></li>
                    <li>Dashboard</li>
                    <li>Users</li>
                    <li>Settings</li>
                </ul>
            </nav>
        </div>
        <div class="LowerHeader">
             <nav>
                <ul>
                    <li>Home</li>
                    <li>Dashboard</li>
                </ul>
            </nav>

        </div>
    </div>
</template>

<style scoped>

    nav ul {
        display: flex;
        list-style: none;
        position: relative;
        left: -20px;
    }
    nav ul li {
        margin-left: 10px;
        cursor: pointer;
    }

    .UpperHeader nav ul li{
        position: relative;
        left: -20px;
        margin-left: 30px;
        
    }

    .LowerHeader {
        border-top: 3px solid #f3f4f5 ;
    }

</style>