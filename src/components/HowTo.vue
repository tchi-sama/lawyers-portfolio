<template>
    <div class="container mx-auto my-10 py-8">
        <h1 class="text-4xl py-4 font-bold">كيفية الاستفادة من خدمات المفوض القضائي</h1>
        <p>الخطوات الواجب اتباعها للاستفادة من خدمات المفوض القضائي</p>
        <div class="flex gap-4 pt-8">
            <div class="p-8 rounded-xl flex flex-col gap-3 bg-white shadow-lg" v-for="(step, i) in steps" :key="i">
                <h1 class="text-6xl text-gray-400">0{{ i + 1 }}</h1>
                <h3 class="text-2xl font-bold">{{ step.name }}</h3>
                <p>{{ step.description }}</p>
            </div>
        </div>
        <button class="btn bg-red-500 my-8 hover:bg-red-600 text-white">احجز موعد</button>
        <div class="bg-white p-8 rounded-xl shadow-xl  max-w-lg">
            <h3 class="text-xl pb-4">مراكش</h3>
            <p>ذ. رشيد لبرود</p>
            <p>شارع علال الفاسي، مركب الدار الحمراء، عمارة س الطابق 2 رقم 8</p>
            <p>993 535 667 212+</p>
            <h3 class="text-red-400 font-bold pt-4"> الموقع على الخريطة</h3>
        </div>
    </div>
</template>
<script>
export default {
    name: "HowTo",
    data() {
        return {
            steps: [
                { name: "حجز الموعد", description: "يمكنكم حجز موعد على موقعنا الإلكتروني، أو الاتصال بنا على الرقم التالي993 535 667 212+" },
                { name: "تحديدالمشكل", description: "بعد حجز الموعد، تفضلو بزيارتنا في مكتبنا لمناقشة التفاصيل والتعرف على المشكل." },
                { name: "الشروع في العمل", description: "سيسمح لنا تحديد احتياجاتكم بصفة دقيقة ببدء العمل و التنفيد المباشر للإجراءات اللازمة." },
            ]
        }
    }
}
</script>