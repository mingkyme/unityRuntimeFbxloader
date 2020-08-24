## chinese
一个Unity插件，用来运行时读取fbx。
现在支持静态mesh读取，支持自带贴图导入（不支持tga格式）
## korean
적용 방법

1. Unity Assets 폴더 안에 Plugins 폴더를 생성한다.
2. Plugins 폴더 안에 fbxImporter.dll, Jhqc.UnityFbxLoader.dll, protobuf-net.dll 넣는다.
3. Unity Assets 폴더 안에 Scripts 폴더를 만든다.
4. Scripts 폴더 안에 FbxLoader.cs 파일을 넣는다.
5. 새 스크립트르 생성하여 아래와 같이 사용한다.
```cs
void Start()
    {
        GameObject go = new GameObject();
        FbxLoader.InitLoader();
        print(FbxLoader.LoadFbx("c:\\b.fbx", out go));
    }
```
