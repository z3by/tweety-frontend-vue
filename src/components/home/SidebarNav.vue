<template>
    <nav class="w-[68px] xl:w-64">
        <ul>
            <NavItem text="Home" to="/home">
                <template v-slot:prefix="props">
                    <HomeIconFill class="inline h-6" v-if="props.active" />
                    <HomeIconOutline class="inline h-6" v-else />
                </template>
            </NavItem>
            <NavItem text="Explore" to="/explore">
                <template v-slot:prefix="props">
                    <ExploreIconFill class="inline h-6" v-if="props.active" />
                    <ExploreIconOutline class="inline h-6" v-else />
                </template>
            </NavItem>
            <NavItem text="Notifications" to="/notifications">
                <template v-slot:prefix="props">
                    <NotificationsIconFill class="inline h-6" v-if="props.active" />
                    <NotificationsIconOutline class="inline h-6" v-else />
                </template>
            </NavItem>
            <NavItem text="Messages" to="/messages">
                <template v-slot:prefix="props">
                    <MessagesIconFill class="inline h-6" v-if="props.active" />
                    <MessagesIconOutline class="inline h-6" v-else />
                </template>
            </NavItem>

            <NavItem text="Bookmarks" to="/bookmarks">
                <template v-slot:prefix="props">
                    <BookmarksIconFill class="inline h-6" v-if="props.active" />
                    <BookmarksIconOutline class="inline h-6" v-else />
                </template>
            </NavItem>
            <NavItem text="Lists" to="/lists">
                <template v-slot:prefix="props">
                    <ListsIconFill class="inline h-6" v-if="props.active" />
                    <ListsIconOutline class="inline h-6" v-else />
                </template>
            </NavItem>
            <NavItem text="Profile" to="/profile">
                <template v-slot:prefix="props">
                    <ProfileIconFill class="inline h-6" v-if="props.active" />
                    <ProfileIconOutline class="inline h-6" v-else />
                </template>
            </NavItem>
            <NavItem text="More">
                <template v-slot:prefix>
                    <MoreIcon class="inline h-6" />
                </template>
            </NavItem>
        </ul>
    </nav>
</template>
