using System.Collections;
using System.Collections.Generic;
using Unity.VisualScripting.Dependencies.NCalc;
using UnityEngine;
using UnityEngine.UI;
using TMPro;


public class CoinCollection : MonoBehaviour
{
    public TMP_Text coinText; // UI para mostrar la cantidad de monedas
    private int coinCount = 0; // Contador de monedas

    // Se ejecuta cuando un objeto entra en el trigger
    private void OnTriggerEnter(Collider other)
    {
        if (other.CompareTag("Player")) // Verifica si es el jugador
        {
            coinCount++; // Suma 1 al contador
            coinText.text = coinCount.ToString(); // Actualiza el texto en la UI

            Destroy(gameObject); // Elimina la moneda después de recogerla
        }
    }
}
