repo1
https://gist.github.com/d4c3f2de345d15be5e01

ESTE ES EL XML DE LA PRIMERA ACTIVIDAD QUE PODRIA APARECER EN LA APLICACION
TIENE UNA IMAGEN Y UNA BARRA DE PROGRESA MIENTRAS CARGA EL INICIO DE LA APLICACION, PODRIA SER MIENTRAS CARGA EL GPS

    <RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent" 
    >
    
    <!-- ESTE ES EL LAYOUT QUE CONTIENE LA IMAGEN EN LA MITAD SUPERIOR DE LA PANTALLA -->
    <!-- El nombre de la imagen es ic_cargando y esta en la carpeta res/drawableS -->
    <LinearLayout
        android:id="@+id/layoutalto"
        android:orientation="vertical"
      android:layout_width="wrap_content"
    	android:layout_height="match_parent" 
    	android:gravity="top"
    	android:background="@drawable/ic_cargando"
    	android:layout_marginBottom="250dp"
        >
    </LinearLayout>
    
    <!-- ESTE LAYOUT CONTIENE LA BARRA DE PROGRESO Y EL TEXTO DE LA MITAD INFERIOR DE LA PANTALLA -->
    <LinearLayout
        android:id="@+id/layoutbajo"
        android:orientation="vertical"
    	android:layout_width="fill_parent"
    	android:layout_height="wrap_content"    	
    	android:gravity="bottom"
    	android:layout_marginTop="210dp"
    	
        >

        <ProgressBar
            android:id="@+id/progressBar1"
            style="?android:attr/progressBarStyleLarge"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content" 
            android:layout_marginTop="90dp"
            android:layout_marginLeft="120dp"
            
            
            />

        <!-- La variable load la es declarada en la clase strings.xml -->
        <TextView
            android:id="@+id/textView1"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="@string/load" 
            android:layout_marginLeft="130dp"/>

    </LinearLayout>

</RelativeLayout>
