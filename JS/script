// Menghubungkan form dengan event listener
document.getElementById("temperatureForm").addEventListener("submit", function (e) {
    e.preventDefault(); // Mencegah pengiriman form default

    // Mengambil nilai suhu dalam Celsius dari input
    const celsiusInput = parseFloat(document.getElementById("temperature").value);

    if (!isNaN(celsiusInput)) {
        // Menghitung konversi suhu
        const fahrenheitResult = celsiusToFahrenheit(celsiusInput);

        // Menampilkan hasil konversi
        displayResult(celsiusInput, fahrenheitResult);
    } else {
        alert("Masukkan suhu yang valid dalam bentuk angka.");
    }
});

// Fungsi untuk menghitung konversi suhu dari Celsius ke Fahrenheit
function celsiusToFahrenheit(celsius) {
    return (celsius * 9/5) + 32;
}

// Fungsi untuk menampilkan hasil konversi
function displayResult(celsius, fahrenheit) {
    document.getElementById("celsiusResult").textContent = "Celsius: " + celsius + "°C";
    document.getElementById("fahrenheitResult").textContent = "Fahrenheit: " + fahrenheit + "°F";
    document.getElementById("rumus").textContent = "Rumus : " + "(" + celsius + "*" + "9/5" + ")" + "+" + "32" + "=" + fahrenheit;
}

// Ambil elemen-elemen yang diperlukan
const temperatureForm = document.getElementById("temperatureForm");
const temperatureInput = document.getElementById("temperature");
const celsiusResult = document.getElementById("celsiusResult");
const fahrenheitResult = document.getElementById("fahrenheitResult");
const rumus = document.getElementById("rumus");

// Simpan nilai awal input suhu
const initialTemperature = temperatureInput.value;

// Fungsi untuk mereset tampilan ke nilai awal
function resetForm() {
    temperatureInput.value = initialTemperature;
    celsiusResult.textContent = "Celsius: ";
    fahrenheitResult.textContent = "Fahrenheit: ";
    rumus.textContent = "Rumus :"
}

// Tambahkan event listener ke tombol Reset
const resetButton = document.getElementById("resetButton");
resetButton.addEventListener("click", resetForm);

