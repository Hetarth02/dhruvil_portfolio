<script lang="ts">
    import php from '$lib/assets/images/skills/php.svg';
    import python from '$lib/assets/images/skills/python.svg';
    import html from '$lib/assets/images/skills/html.svg';
    import css from '$lib/assets/images/skills/css.svg';
    import scss from '$lib/assets/images/skills/scss.svg';
    import js from '$lib/assets/images/skills/js.svg';
    import ts from '$lib/assets/images/skills/ts.svg';
    import sql from '$lib/assets/images/skills/sql.svg';
    import nosql from '$lib/assets/images/skills/nosql.svg';
    import adonis from '$lib/assets/images/skills/adonis.svg';
    import laravel from '$lib/assets/images/skills/laravel.svg';
    import nodejs from '$lib/assets/images/skills/nodejs.svg';
    import sveltekit from '$lib/assets/images/skills/sveltekit.svg';
    import vuejs from '$lib/assets/images/skills/vuejs.svg';
    import reactjs from '$lib/assets/images/skills/reactjs.svg';
    import socketio from '$lib/assets/images/skills/socketio.svg';
    import aws from '$lib/assets/images/skills/aws.svg';
    import azure from '$lib/assets/images/skills/azure.svg';
    import gcp from '$lib/assets/images/skills/gcp.svg';
    import postgresql from '$lib/assets/images/skills/postgresql.svg';
    import mysql from '$lib/assets/images/skills/mysql.svg';
    import mongodb from '$lib/assets/images/skills/mongodb.svg';
    import heroku from '$lib/assets/images/skills/heroku.svg';
    import netlify from '$lib/assets/images/skills/netlify.svg';
    import vercel from '$lib/assets/images/skills/vercel.svg';
    import linux from '$lib/assets/images/skills/linux.svg';
    import terraform from '$lib/assets/images/skills/terraform.svg';
    import docker from '$lib/assets/images/skills/docker.svg';
    import vs_code from '$lib/assets/images/skills/vs_code.svg';
    import git from '$lib/assets/images/skills/git.svg';
    import bitbucket from '$lib/assets/images/skills/bitbucket.svg';
    import postman from '$lib/assets/images/skills/postman.svg';

    const skills: Record<string, Record<string, string>[]> = {
        'Techniques & Instruments': [
            {
                title: 'XRF',
                icon: php
            },
            {
                title: 'XRD',
                icon: python
            },
            {
                title: 'AAS',
                icon: html
            },
            {
                title: 'ICP-MS',
                icon: scss
            },
            {
                title: 'Wet Chemistry',
                icon: css
            }
            // {
            //     title: 'Javascript',
            //     icon: js
            // },
            // {
            //     title: 'TypeScript',
            //     icon: ts
            // },
            // {
            //     title: 'SQL',
            //     icon: sql
            // },
            // {
            //     title: 'NoSQL',
            //     icon: nosql
            // }
        ],
        // Software: [
        //     {
        //         title: 'AdonisJs',
        //         icon: adonis
        //     },
        //     {
        //         title: 'Laravel',
        //         icon: laravel
        //     },
        //     {
        //         title: 'NodeJs',
        //         icon: nodejs
        //     },
        //     {
        //         title: 'Sveltekit',
        //         icon: sveltekit
        //     },
        //     {
        //         title: 'VueJs',
        //         icon: vuejs
        //     },
        //     {
        //         title: 'ReactJs',
        //         icon: reactjs
        //     },
        //     {
        //         title: 'Socket.IO',
        //         icon: socketio
        //     }
        // ],
        'Fields of Expertise': [
            {
                title: 'Analytical Chemistry',
                icon: aws
            },
            {
                title: 'Mineralogy',
                icon: azure
            },
            {
                title: 'Combustion Additives',
                icon: gcp
            },
            {
                title: 'Rare Earth Elements',
                icon: postgresql
            }
            // {
            //     title: 'MySQL',
            //     icon: mysql
            // },
            // {
            //     title: 'MongoDB',
            //     icon: mongodb
            // },
            // {
            //     title: 'Heroku',
            //     icon: heroku
            // },
            // {
            //     title: 'Netlify',
            //     icon: netlify
            // },
            // {
            //     title: 'Vercel',
            //     icon: vercel
            // }
        ]
        // 'Developer Tools': [
        //     {
        //         title: 'Linux',
        //         icon: linux
        //     },
        //     {
        //         title: 'Terraform',
        //         icon: terraform
        //     },
        //     {
        //         title: 'Docker',
        //         icon: docker
        //     },
        //     {
        //         title: 'VS Code',
        //         icon: vs_code
        //     },
        //     {
        //         title: 'Git/Github',
        //         icon: git
        //     },
        //     {
        //         title: 'Bitbucket',
        //         icon: bitbucket
        //     },
        //     {
        //         title: 'Postman',
        //         icon: postman
        //     }
        // ]
    };
</script>

<div class="space-y-4 md:space-y-10">
    <!-- Info -->
    <div class="space-y-4 text-center">
        <h2 class="h2">Skills I know...</h2>
    </div>

    <div class="w-11/12 mx-auto flex flex-col justify-between items-center gap-4">
        {#each Object.keys(skills) as category}
            <div class="flex flex-col md:flex-row items-center gap-2 w-full">
                <div
                    class="card variant-glass p-2 shadow-lg text-center w-[10rem] sm:flex sm:flex-col sm:justify-center sm:items-center"
                    title="feature"
                >
                    <h3>{category}</h3>
                </div>
                <div
                    class="flex flex-row flex-wrap justify-center md:justify-start items-center gap-2 w-full"
                >
                    |
                    {#each skills[category] as feature}
                        <div class="block">
                            <span>{feature.title} | </span>
                        </div>
                    {/each}
                </div>
            </div>
        {/each}
    </div>
</div>
