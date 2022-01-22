<template>
    <div class="bg-[#021627] p-16 rounded-md text-gray-default text-18" style="font-family: monospace">
        <p>
            # Tech Stack
        </p>
        <p>
            ## Web
        </p>
        <p>
            tailwindcss / vue / twig / c#
        </p>
        <br>
        <p>
            ## MX Reality & 3D
        </p>
        <p>
            unity / steamvr / vuforia / blender 
        </p>
        <br>
        <p>
            ## Design & UI
        </p>
        <p>
            adobe xd / photoshop 
        </p>
    </div>
</template>
<script>
export default {
    name: "TechStack",
    data () {
        return {
            publicPath: process.env.BASE_URL
        }
    }
}
</script>