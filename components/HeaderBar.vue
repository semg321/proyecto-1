<template>
    <header class="header-bar d-flex align-items-center bg-dark">
        <nav class="navbar container-fluid d-flex justify-content-between align-items-center">
            <form class="d-flex" role="search">
                <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
                <button class="btn btn-outline-success d-flex align-items-center" type="submit">
                    <Icon name="iconamoon:search-fill" size="24px" />
                </button>
            </form>
            <div class="user-link d-flex align-items-center justify-content-center">
                <NuxtLink to="/login/">
                    <Icon name="fa6-regular:user" size="40px" class="user-icon"/>
                </NuxtLink>
            </div>
        </nav>
    </header>
</template>

<style scoped>
.header-bar {
    height: 100px;
    width: 100%;
    top: 0;
    border-radius: 10px;
    z-index: 1000;
}

.navbar {
    margin: 0 25px;
}

.btn {
    border: solid 2px;
    color: white;
}

.user-link {
    cursor: pointer;
    display: flex;
    align-items: center;
    justify-content: center;
    width: 40px;
    height: 40px;
}

.user-icon {
    color: white;
    transition: box-shadow 0.3s ease-in-out;
}


.user-icon:hover {
    box-shadow: 0px 0px 20px white;
}

.me-2 {
    margin-right: 0.5rem;
}
</style>
