paquete com.ejemplo.admintareas

importar android.os.Bundle
importar androidx.activity.ComponentActivity
importar androidx.activity.compose.setContent
importar androidx.compose.foundation.Image
importar androidx.compose.foundation.layout.Column
importar androidx.compose.foundation.layout.fillMaxSize
Importar androidx.compose.foundation.layout.padding
importar androidx.compose.material.MaterialTheme
importar androidx.compose.material.Surface
importar androidx.compose.material.Text
importar androidx.compose.runtime.Composable
importar androidx.compose.ui.Modifier
import androidx.compose.ui.modifier.modifierLocalConsumer
import androidx.compose.ui.res.painterResource
importar androidx.compose.ui.text.style.TextAlign
import androidx.compose.ui.tooling.preview.Preview
importar androidx.compose.ui.unit.dp
import com.example.admintareas.ui.theme.AdminTareasTheme

class MainActivity : ComponentActivity() {
    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        setContent{
            PersonalData(name = "Gabriela")
        }
    }

    @Composable
    diversión privada  PersonalData(nombre: String){

        Columna(
 modificador = Modificador.padding(100.dp)
        ) {
            Imagen(
 pintor = pintorRecurso(R.drawable.logo2),
 contentDescription = null )
            val Justify: TextAlign
            Text(text ="\n"+ " Todas las tareas completadas  " + "\n")
            Text(text = "¡Buen trabajo!"  + "\n")
        }
    }



}