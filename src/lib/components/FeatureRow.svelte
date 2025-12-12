<script lang="ts">
    export let title: string;
    export let description: string;
    export let image: string;
    export let icon: string;

    // Extract the bold part of the description (first sentence)
    $: splitDesc = description.split('. ');
    $: boldDesc = splitDesc[0] + '.';
    $: restDesc = splitDesc.slice(1).join('. ');
</script>

<div class="bg-[#F3F4F6] rounded-3xl p-8 md:p-12 transition-all hover:bg-gray-200 group">
    <!-- Header -->
    <div class="flex items-center gap-3 mb-8">
        <div class="text-[var(--color-ifirma-primary)]">
            {#if icon === 'camera'}
                <svg class="w-6 h-6" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M23 19a2 2 0 0 1-2 2H3a2 2 0 0 1-2-2V8a2 2 0 0 1 2-2h4l2-3h6l2 3h4a2 2 0 0 1 2 2z"></path><circle cx="12" cy="13" r="4"></circle></svg>
            {:else if icon === 'electric'}
                <svg class="w-6 h-6" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M13 2L3 14h9l-1 8 10-12h-9l1-8z"></path></svg>
            {:else if icon === 'certificate'}
                <svg class="w-6 h-6" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"></path><polyline points="14 2 14 8 20 8"></polyline><line x1="16" y1="13" x2="8" y2="13"></line><line x1="16" y1="17" x2="8" y2="17"></line><polyline points="10 9 9 9 8 9"></polyline></svg>
            {:else if icon === 'floorplan'}
                <svg class="w-6 h-6" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect x="3" y="3" width="18" height="18" rx="2" ry="2"></rect><line x1="3" y1="9" x2="21" y2="9"></line><line x1="9" y1="21" x2="9" y2="9"></line></svg>
            {:else if icon === 'virtual'}
                <svg class="w-6 h-6" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><circle cx="12" cy="12" r="10"></circle><polygon points="10 8 16 12 10 16 10 8"></polygon></svg>
            {:else if icon === 'docs'}
                <svg class="w-6 h-6" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"></path><polyline points="14 2 14 8 20 8"></polyline><line x1="16" y1="13" x2="8" y2="13"></line><line x1="16" y1="17" x2="8" y2="17"></line><line x1="10" y1="9" x2="8" y2="9"></line></svg>
            {/if}
        </div>
        <h3 class="text-xl font-semibold text-gray-900">{title}</h3>
    </div>

    <!-- Image Placeholder / Abstract UI -->
    <div class="bg-white rounded-xl shadow-sm border border-gray-200 overflow-hidden mb-8 aspect-[16/9] relative group-hover:shadow-md transition-shadow">
        {#if image === 'photography'}
            <!-- Photography UI -->
            <div class="p-6 h-full flex items-center justify-center bg-gradient-to-br from-gray-50 to-gray-100">
                <div class="grid grid-cols-3 gap-2 w-full">
                    <div class="aspect-square bg-gray-300 rounded-lg"></div>
                    <div class="aspect-square bg-gray-400 rounded-lg"></div>
                    <div class="aspect-square bg-gray-300 rounded-lg"></div>
                    <div class="aspect-square bg-gray-400 rounded-lg"></div>
                    <div class="aspect-square bg-gray-500 rounded-lg"></div>
                    <div class="aspect-square bg-gray-300 rounded-lg"></div>
                </div>
            </div>
        {:else if image === 'inspection'}
            <!-- Inspection UI -->
            <div class="p-6 h-full flex flex-col justify-center">
                <div class="space-y-4">
                    <div class="flex items-center gap-3">
                        <div class="w-8 h-8 rounded-full bg-green-100 flex items-center justify-center">
                            <svg class="w-4 h-4 text-green-600" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path></svg>
                        </div>
                        <div class="flex-1">
                            <div class="h-2 bg-gray-200 rounded w-3/4"></div>
                            <div class="h-1.5 bg-gray-100 rounded w-1/2 mt-1"></div>
                        </div>
                    </div>
                    <div class="flex items-center gap-3">
                        <div class="w-8 h-8 rounded-full bg-green-100 flex items-center justify-center">
                            <svg class="w-4 h-4 text-green-600" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path></svg>
                        </div>
                        <div class="flex-1">
                            <div class="h-2 bg-gray-200 rounded w-2/3"></div>
                            <div class="h-1.5 bg-gray-100 rounded w-1/3 mt-1"></div>
                        </div>
                    </div>
                    <div class="flex items-center gap-3">
                        <div class="w-8 h-8 rounded-full bg-yellow-100 flex items-center justify-center">
                            <span class="text-yellow-600 text-xs">!</span>
                        </div>
                        <div class="flex-1">
                            <div class="h-2 bg-gray-200 rounded w-4/5"></div>
                            <div class="h-1.5 bg-gray-100 rounded w-2/3 mt-1"></div>
                        </div>
                    </div>
                </div>
            </div>
        {:else if image === 'epc'}
            <!-- EPC Certificate UI -->
            <div class="p-6 h-full flex items-center justify-center bg-gradient-to-br from-green-50 to-red-50">
                <div class="w-full max-w-xs">
                    <div class="text-xs font-bold mb-2 text-gray-700">Energy Performance</div>
                    <div class="space-y-1">
                        {#each [{label: 'A++', color: 'bg-green-600', width: 'w-1/6'}, {label: 'A+', color: 'bg-green-500', width: 'w-1/4'}, {label: 'A', color: 'bg-green-400', width: 'w-1/3'}, {label: 'B', color: 'bg-yellow-400', width: 'w-1/2'}, {label: 'C', color: 'bg-yellow-500', width: 'w-2/3'}, {label: 'D', color: 'bg-orange-400', width: 'w-3/4'}, {label: 'E', color: 'bg-red-400', width: 'w-5/6'}] as rating}
                            <div class="flex items-center gap-2">
                                <span class="text-xs font-bold w-8">{rating.label}</span>
                                <div class="{rating.color} {rating.width} h-4 rounded-r"></div>
                            </div>
                        {/each}
                    </div>
                </div>
            </div>
        {:else if image === 'floorplan'}
            <!-- Floor Plan UI -->
            <div class="p-6 h-full bg-white">
                <div class="border-2 border-gray-300 h-full rounded relative">
                    <div class="absolute top-4 left-4 right-1/2 bottom-1/2 border-2 border-gray-300 bg-gray-50 flex items-center justify-center text-xs text-gray-500">Living</div>
                    <div class="absolute top-4 left-1/2 right-4 bottom-1/2 border-2 border-gray-300 bg-gray-50 flex items-center justify-center text-xs text-gray-500">Kitchen</div>
                    <div class="absolute top-1/2 left-4 right-1/2 bottom-4 border-2 border-gray-300 bg-gray-50 flex items-center justify-center text-xs text-gray-500">Bedroom</div>
                    <div class="absolute top-1/2 left-1/2 right-4 bottom-4 border-2 border-gray-300 bg-gray-50 flex items-center justify-center text-xs text-gray-500">Bath</div>
                </div>
            </div>
        {:else if image === 'virtual'}
            <!-- Virtual Tour UI -->
            <div class="p-6 h-full flex items-center justify-center bg-gray-900 relative overflow-hidden">
                <div class="absolute inset-0 bg-gradient-to-br from-blue-900/30 to-purple-900/30"></div>
                <div class="relative z-10 text-center">
                    <div class="w-16 h-16 mx-auto mb-3 rounded-full bg-white/20 backdrop-blur-sm flex items-center justify-center">
                        <svg class="w-8 h-8 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24"><circle cx="12" cy="12" r="10"></circle><polygon points="10 8 16 12 10 16 10 8"></polygon></svg>
                    </div>
                    <div class="text-white text-sm font-medium">360° Virtual Tour</div>
                </div>
            </div>
        {:else if image === 'documentation'}
            <!-- Documentation UI -->
            <div class="p-6 h-full flex flex-col">
                <div class="flex items-center justify-between mb-4 pb-3 border-b border-gray-200">
                    <span class="text-sm font-bold text-gray-800">Property Documents</span>
                    <span class="text-xs text-green-600 bg-green-50 px-2 py-1 rounded-full">Complete</span>
                </div>
                <div class="space-y-2">
                    {#each ['Photos', 'Floor Plans', 'EPC Certificate', 'Electrical Report', 'Virtual Tour'] as doc}
                        <div class="flex items-center gap-2 text-xs text-gray-600">
                            <svg class="w-4 h-4 text-green-500" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path></svg>
                            <span>{doc}</span>
                        </div>
                    {/each}
                </div>
            </div>
        {:else if image === 'collateral'}
            <!-- Collateral UI -->
            <div class="p-6 h-full flex flex-col">
                <div class="flex justify-between items-center mb-6 border-b border-gray-100 pb-4">
                    <div class="font-bold text-gray-800">Collateral</div>
                    <div class="flex gap-2">
                        <div class="w-20 h-8 bg-gray-100 rounded"></div>
                    </div>
                </div>
                <div class="space-y-3">
                    <div class="flex justify-between text-xs text-gray-400 uppercase tracking-wider">
                        <span>Collateral Type</span>
                        <span>Value</span>
                        <span>Status</span>
                    </div>
                    {#each [1, 2, 3] as i}
                    <div class="flex justify-between items-center py-2 border-b border-gray-50">
                        <div class="w-24 h-4 bg-gray-100 rounded"></div>
                        <div class="w-16 h-4 bg-gray-100 rounded"></div>
                        <div class="w-12 h-4 bg-green-100 text-green-600 rounded-full text-[10px] flex items-center justify-center">Active</div>
                    </div>
                    {/each}
                </div>
            </div>
        {:else if image === 'connect'}
            <!-- Connect UI -->
            <div class="p-6 h-full flex flex-col items-center justify-center bg-gray-50">
                <div class="bg-white p-4 rounded-lg shadow-sm border border-gray-200 w-3/4">
                    <div class="flex items-center gap-3 mb-4">
                        <div class="w-8 h-8 rounded-full bg-blue-100 flex items-center justify-center text-blue-600">
                            <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z"></path></svg>
                        </div>
                        <div class="text-sm font-medium">Payment Received Webhook</div>
                    </div>
                    <div class="h-px bg-gray-100 w-full mb-4"></div>
                    <div class="flex justify-center">
                        <div class="bg-gray-100 text-gray-500 text-xs px-2 py-1 rounded">Branch on due date</div>
                    </div>
                </div>
            </div>
        {:else if image === 'data'}
            <!-- Data UI -->
            <div class="p-6 h-full flex flex-col">
                <div class="flex gap-4 mb-6">
                    <div class="w-1/2 p-4 bg-gray-50 rounded-lg border border-gray-100">
                        <div class="text-xs text-gray-400 mb-1">Avg. min. pay cents</div>
                        <div class="text-xl font-bold text-gray-900">333.33</div>
                        <div class="mt-4 h-16 flex items-end gap-1">
                            {#each [40, 60, 30, 70, 50, 80] as h}
                                <div class="w-full bg-blue-200 rounded-t" style="height: {h}%"></div>
                            {/each}
                        </div>
                    </div>
                    <div class="w-1/2 p-4 bg-gray-50 rounded-lg border border-gray-100">
                        <div class="text-xs text-gray-400 mb-1">Average balance</div>
                        <div class="text-xl font-bold text-gray-900">$3,183.48</div>
                         <div class="mt-4 h-2 bg-gray-200 rounded-full overflow-hidden">
                            <div class="h-full bg-blue-500 w-2/3"></div>
                        </div>
                    </div>
                </div>
            </div>
        {:else if image === 'lab'}
            <!-- Lab UI -->
            <div class="p-6 h-full bg-white">
                <div class="font-mono text-xs text-gray-400 mb-4">Action Timeline</div>
                <div class="space-y-4 relative pl-4 border-l border-gray-200">
                    <div class="relative">
                        <div class="absolute -left-[21px] top-1 w-3 h-3 rounded-full bg-green-500 border-2 border-white"></div>
                        <div class="text-xs font-medium text-gray-900">Cycle 1: Dec 13 12:43PM - 15 Dec @ 00:00AM</div>
                        <div class="mt-1 text-xs text-gray-500 pl-2 border-l border-gray-100 ml-1">Automation: Account Created</div>
                    </div>
                     <div class="relative">
                        <div class="absolute -left-[21px] top-1 w-3 h-3 rounded-full bg-green-500 border-2 border-white"></div>
                        <div class="text-xs font-medium text-gray-900">Minimum Payment</div>
                         <div class="mt-1 text-xs text-gray-500 pl-2 border-l border-gray-100 ml-1">Automation: Generate Statement</div>
                    </div>
                </div>
            </div>
        {:else if image === 'preview'}
            <!-- Preview UI -->
            <div class="p-6 h-full">
                <table class="w-full text-xs">
                    <thead>
                        <tr class="text-gray-400 border-b border-gray-100">
                            <th class="text-left pb-2 font-normal">Action</th>
                            <th class="text-right pb-2 font-normal">Current</th>
                            <th class="text-right pb-2 font-normal">Preview</th>
                        </tr>
                    </thead>
                    <tbody class="text-gray-600">
                        <tr class="border-b border-gray-50">
                            <td class="py-2">Account Status</td>
                            <td class="py-2 text-right text-red-500">Suspended</td>
                            <td class="py-2 text-right text-green-500">Active</td>
                        </tr>
                         <tr class="border-b border-gray-50">
                            <td class="py-2">Minimum Payment</td>
                            <td class="py-2 text-right">$2,950.00</td>
                            <td class="py-2 text-right">$0.00</td>
                        </tr>
                         <tr>
                            <td class="py-2">Total Balance</td>
                            <td class="py-2 text-right">$5,925.00</td>
                            <td class="py-2 text-right">$2,975.00</td>
                        </tr>
                    </tbody>
                </table>
            </div>
        {:else if image === 'guard'}
            <!-- Guard UI -->
            <div class="p-6 h-full flex flex-col justify-center">
                <div class="text-xs text-gray-400 mb-2">Customer ID: 42784724728</div>
                <div class="grid grid-cols-2 gap-4">
                    <div class="p-3 bg-green-50 rounded border border-green-100">
                        <div class="text-[10px] text-green-600 uppercase">Account status</div>
                        <div class="text-sm font-bold text-green-700">Active</div>
                    </div>
                    <div class="p-3 bg-red-50 rounded border border-red-100">
                        <div class="text-[10px] text-red-600 uppercase">Account substatus</div>
                        <div class="text-sm font-bold text-red-700">Delinquent</div>
                    </div>
                </div>
                <div class="grid grid-cols-2 gap-4 mt-4">
                    <div>
                        <div class="text-[10px] text-gray-400 uppercase">Missed payments</div>
                        <div class="text-lg font-bold">3</div>
                    </div>
                     <div>
                        <div class="text-[10px] text-gray-400 uppercase">Payment frequency</div>
                        <div class="text-lg font-bold">1</div>
                    </div>
                </div>
            </div>
        {/if}
    </div>

    <!-- Footer -->
    <div class="flex items-end justify-between gap-4">
        <div class="max-w-xl">
            <p class="text-gray-900 text-lg leading-relaxed">
                <span class="font-bold">{boldDesc}</span> <span class="text-gray-600">{restDesc}</span>
            </p>
        </div>
        <button class="w-10 h-10 rounded-full border border-gray-300 flex items-center justify-center text-gray-600 hover:bg-black hover:text-white hover:border-black transition-colors flex-shrink-0">
            <svg class="w-4 h-4" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                <line x1="7" y1="17" x2="17" y2="7"></line>
                <polyline points="7 7 17 7 17 17"></polyline>
            </svg>
        </button>
    </div>
</div>
