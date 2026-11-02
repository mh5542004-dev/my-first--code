<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ethiopia Vehicle & Bajaj Tax Portal</title>
    <!-- Tailwind CSS Engine for lightweight design -->
    <script src="https://tailwindcss.com"></script>
</head>
<body class="bg-gray-50 font-sans text-gray-900">

    <!-- Header Navigation -->
    <header class="bg-emerald-800 text-white shadow-md p-4">
        <div class="container mx-auto flex justify-between items-center">
            <h1 class="text-xl font-bold tracking-wide">የኢትዮጵያ ትራንስፖርት ባለስልጣን | Tax System</h1>
            <span class="bg-emerald-700 text-xs px-3 py-1.5 rounded-full border border-emerald-500">Connected to Fayda ID</span>
        </div>
    </header>

    <!-- Main Container Layout -->
    <main class="container mx-auto my-8 p-4 grid grid-cols-1 lg:grid-cols-3 gap-8">
        
        <!-- Interactive Portal Form -->
        <section class="lg:col-span-2 bg-white rounded-xl shadow p-6 border border-gray-100">
            <h2 class="text-lg font-semibold border-b pb-3 mb-6 text-gray-800">New Registration & Tax Assessment</h2>
            
            <form class="space-y-6">
                <!-- Row 1 -->
                <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                    <div>
                        <label class="block text-sm font-medium text-gray-700 mb-1">Plate Number</label>
                        <input type="text" placeholder="e.g., AA-2-B99999" class="w-full border border-gray-300 rounded-md p-2.5 focus:ring-2 focus:ring-emerald-500 focus:outline-none">
                    </div>
                    <div>
                        <label class="block text-sm font-medium text-gray-700 mb-1">Owner Fayda ID</label>
                        <input type="text" placeholder="ET-123456789-X" class="w-full border border-gray-300 rounded-md p-2.5 focus:ring-2 focus:ring-emerald-500 focus:outline-none">
                    </div>
                </div>

                <!-- Row 2 -->
                <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                    <div>
                        <label class="block text-sm font-medium text-gray-700 mb-1">Vehicle Classification</label>
                        <select class="w-full border border-gray-300 rounded-md p-2.5 bg-white focus:ring-2 focus:ring-emerald-500 focus:outline-none">
                            <option value="Standard">Standard Automobile (Code 2 / Code 3)</option>
                            <option value="Bajaj">Three-Wheeler Bajaj</option>
                        </select>
                    </div>
                    <div>
                        <label class="block text-sm font-medium text-gray-700 mb-1">Operational Region</label>
                        <select class="w-full border border-gray-300 rounded-md p-2.5 bg-white focus:ring-2 focus:ring-emerald-500 focus:outline-none">
                            <option>Addis Ababa</option>
                            <option>Oromia</option>
                            <option>Amhara</option>
                            <option>Sidama</option>
                        </select>
                    </div>
                </div>

                <!-- Conditional Parameters Box -->
                <div class="p-4 bg-gray-50 rounded-lg border border-dashed border-gray-200 grid grid-cols-1 md:grid-cols-2 gap-4">
                    <div>
                        <label class="block text-xs font-semibold text-gray-500 uppercase tracking-wider mb-1">Engine Size (cc) - Standard Only</label>
                        <input type="number" placeholder="e.g., 1600" class="w-full border border-gray-300 rounded-md p-2 bg-white text-sm">
                    </div>
                    <div>
                        <label class="block text-xs font-semibold text-gray-500 uppercase tracking-wider mb-1">Cooperative Union/Route - Bajaj Only</label>
                        <input type="text" placeholder="e.g., Bole Sub-City Zone 3" class="w-full border border-gray-300 rounded-md p-2 bg-white text-sm">
                    </div>
                </div>

                <button type="button" class="w-full bg-emerald-700 hover:bg-emerald-800 text-white font-medium py-3 rounded-lg transition-colors shadow">
                    Calculate Dynamic Annual Tax
                </button>
            </form>
        </section>

        <!-- Dynamic Assessment Breakdown Sidebar -->
        <section class="bg-white rounded-xl shadow p-6 border border-gray-100 h-fit space-y-6">
            <h2 class="text-md font-bold text-gray-800 tracking-wide uppercase border-b pb-2">Invoice Summary</h2>
            
            <div class="space-y-3 text-sm">
                <div class="flex justify-between text-gray-600">
                    <span>Base Regional Fee:</span>
                    <span class="font-mono font-semibold text-gray-900">2,500.00 ETB</span>
                </div>
                <div class="flex justify-between text-gray-600">
                    <span>Zonal Route Access Levy:</span>
                    <span class="font-mono font-semibold text-gray-900">200.00 ETB</span>
                </div>
                <div class="flex justify-between text-gray-600">
                    <span>Penalties/Arrears:</span>
                    <span class="font-mono font-semibold text-red-600">0.00 ETB</span>
                </div>
                <div class="border-t pt-3 flex justify-between text-base font-bold text-gray-900">
                    <span>Total Tax Liability:</span>
                    <span class="font-mono text-emerald-800">2,700.00 ETB</span>
                </div>
            </div>

            <!-- Integrated Payments Options Block -->
            <div class="pt-4 border-t space-y-3">
                <span class="block text-xs font-bold text-gray-400 uppercase tracking-wider mb-2">Process Digital Payout</span>
                <button class="w-full flex items-center justify-center space-x-2 border border-blue-500 hover:bg-blue-50 text-blue-700 text-sm font-medium py-2.5 rounded-lg transition">
                    <span>Pay with telebirr</span>
                </button>
                <button class="w-full flex items-center justify-center space-x-2 border border-amber-500 hover:bg-amber-50 text-amber-800 text-sm font-medium py-2.5 rounded-lg transition">
                    <span>Pay via CBE Birr</span>
                </button>
            </div>
        </section>
    </main>

</body>
</html>

