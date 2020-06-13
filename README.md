<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

  <RelativeLayout
      android:id="@+id/toolbar"
      android:layout_width="match_parent"
      android:layout_height="64dp">

      <ImageView
          android:id="@+id/flecha"
          android:layout_width="64dp"
          android:layout_height="64dp"
          android:layout_alignParentStart="true"
          app:srcCompat="@drawable/musixmatch_flecha" />

      <ImageView
          android:id="@+id/opciones"
          android:layout_width="64dp"
          android:layout_height="64dp"
          android:layout_alignParentEnd="true"
          app:srcCompat="@drawable/musixmatch_opciones" />
      
      <LinearLayout
          android:layout_width="match_parent"
          android:layout_height="64dp"
          android:layout_toEndOf="@id/flecha"
          android:layout_toStartOf="@id/opciones"
          android:orientation="vertical">

          <ImageView
              android:layout_width="match_parent"
              android:layout_height="match_parent"
              app:srcCompat="@drawable/musixmatch_cancion" />
      </LinearLayout>
  </RelativeLayout>

    <LinearLayout
        android:id="@+id/musicControls"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:orientation="horizontal"
        android:layout_alignParentBottom="true"
        android:padding="16dp">
        
        <ImageView
            android:layout_width="0dp"
            android:layout_weight="20"
            android:layout_height="wrap_content"
            app:srcCompat="@drawable/musixmatch_caracteristicas" />
        <ImageView
            android:layout_width="0dp"
            android:layout_weight="20"
            android:layout_height="wrap_content"
            app:srcCompat="@drawable/musixmatch_retroceder" />
        <ImageView
            android:layout_width="0dp"
            android:layout_weight="30"
            android:layout_height="wrap_content"
            app:srcCompat="@drawable/musixmatch_play" />
        <ImageView
            android:layout_width="0dp"
            android:layout_weight="20"
            android:layout_height="wrap_content"
            app:srcCompat="@drawable/musixmatch_adelantar" />
        <ImageView
            android:layout_width="0dp"
            android:layout_weight="20"
            android:layout_height="wrap_content"
            app:srcCompat="@drawable/musixmatch_enviar" />
    </LinearLayout>

    <RelativeLayout
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:layout_above="@id/musicControls"
        android:layout_below="@id/toolbar">

        <LinearLayout
            android:id="@+id/details"
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:layout_alignParentBottom="true"
            android:orientation="vertical">

        <RelativeLayout
            android:layout_width="match_parent"
            android:layout_height="wrap_content">

            <ImageView
                android:id="@+id/shuffle"
                android:layout_width="70dp"
                android:layout_height="wrap_content"
                android:layout_alignParentStart="true"
                app:srcCompat="@drawable/musixmatch_shuffle" />

            <ImageView
                android:id="@+id/repeat"
                android:layout_width="70dp"
                android:layout_height="wrap_content"
                android:layout_alignParentEnd="true"
                app:srcCompat="@drawable/musixmatch_repeat" />
        </RelativeLayout>
        <RelativeLayout
            android:layout_width="match_parent"
            android:layout_height="wrap_content">

            <ImageView
                android:id="@+id/tiempoEscuchado"
                android:layout_width="64dp"
                android:layout_height="wrap_content"
                android:layout_alignParentStart="true"
                app:srcCompat="@drawable/musixmatch_tiempoescuchado" />

            <ImageView
                android:id="@+id/tiempoTotal"
                android:layout_width="64dp"
                android:layout_height="wrap_content"
                android:layout_alignParentEnd="true"
                android:layout_marginEnd="7dp"
                app:srcCompat="@drawable/musixmatch_tiempototal" />

            <ImageView
                android:id="@+id/reproductor"
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:layout_toStartOf="@id/tiempoEscuchado"
                android:layout_toEndOf="@id/tiempoTotal"
                app:srcCompat="@drawable/musixmatch_reproductor" />

        </RelativeLayout>
        </LinearLayout>

        <ImageView
            android:layout_width="match_parent"
            android:layout_height="match_parent"
            android:layout_above="@id/details"
            app:srcCompat="@drawable/musixmatch_letra" />
    </RelativeLayout>
</RelativeLayout>
