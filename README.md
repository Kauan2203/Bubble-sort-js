# Bubble-sort-jsfunction bubbleSort(arr) {
    let len = arr.length;
    for (let i = 0; i < len; i++) {
        for (let j = 0; j < len - 1 - i; j++) {
            if (arr[j] > arr[j + 1]) {
                // Trocar os elementos
                let temp = arr[j];
                arr[j] = arr[j + 1];
                arr[j + 1] = temp;
            }
        }
    }
    return arr;
}

// Entrada original
let inputArray = [97, 45, 49, 32, 2, 5, 9, 99, 1, 7];

// Sort
let sortedArray = bubbleSort(inputArray);

// Saída esperada
console.log(sortedArray); // [1, 2, 5, 7, 9, 32, 45, 49, 97, 99]
