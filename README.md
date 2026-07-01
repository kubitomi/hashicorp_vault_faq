# 🔐 HashiCorp Vault - Gyakran Ismételt Kérdések (FAQ)

Üdvözöllek a Vault FAQ repóban! Itt összeszedtük a legfontosabb tudnivalókat.

---

## 📌 Általános Kérdések

<details>
<summary><b>Mi az a Vault "Unsealing" folyamat?</b></summary>

A Vault induláskor **Sealed** (lezárt) állapotban van. Ekkor a titkosított adatok kulcsa (Master Key) szét van darabolva (alapértelmezetten Shamir's Secret Sharing algoritmussal). 
Az **Unsealing** során meg kell adni a minimálisan szükséges számú kulcs-részletet (küszöbérték / threshold), hogy a Vault össze tudja rakni a főkulcsot és elinduljon a működés.
</details>

<details>
<summary><b>Mi a különbség a Token és az AppRole között?</b></summary>

* **Token:** A legalapvetőbb azonosítási mód. Általában emberek vagy rövid életű szkriptek használják.
* **AppRole:** Gépek, mikroszolgáltatások és automatizációk (pl. CI/CD) számára tervezett autentikáció, ami biztonságosabb szerepkör-alapú hozzáférést biztosít.
</details>
