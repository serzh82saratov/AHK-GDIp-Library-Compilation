# AHK GDI+ library compilation.
This is a compilation of user contributed functions for the GDI+ library wrapper made by Tariq Porter [tic] that never made it into.

This repository is a fork of https://github.com/mmikeww/AHKv2-Gdip/ . Some of the newly added functions are possibly not AHK v2 compatible.

This Gdip_all.ahk file should be compatible with projects already relying on the original edition.

The Tutorials/Examples are left untouched. They are the same as in the repository of @mmikeww in Examples folder.
I re-added the original examples in Examples-ahk-v1-1 folder and several new examples that showcase the newly supported GDI+ APIs. These are example scripts initially provided by those that coded the new functions.

# History
- @tic created the original [Gdip.ahk](https://github.com/tariqporter/Gdip/) library
- @Rseding91 updated it to make it compatible with unicode and x64 AHK versions and renamed the file `Gdip_All.ahk`
- @mmikeww's repository updates @Rseding91's `Gdip_All.ahk` to make it compatible with AHK v2 and also fixes some bugs
- this repository attempts to gather all the GDI+ functions contributed by various people that were missing, and further extend the coverage/support of GDI+ API functions

# Comparisions

The following list is comparing Gdip_All.ahk by Tariq Porter and Rseding91 modifications with this new version.

## 18 MODIFIED FUNCTIONS:
- Gdip_CreateBitmapFromClipboard()
- Gdip_SetBitmapToClipboard()
- UpdateLayeredWindow()
- SetImage()
- SetSysColorToControl()
- Gdip_BitmapFromScreen()
- Gdip_BitmapFromHWND()
- Gdip_BitmapFromBRA()
- Gdip_DrawLines()
- Gdip_FillPolygon()
- Gdip_DrawImagePointsRect()
- Gdip_SetImageAttributesColorMatrix()
- Gdip_SaveBitmapToFile()
- Gdip_CreateBitmapFromFile()
- Gdip_TextToGraphics()
- Gdip_GetClipRegion()
- Gdip_CreateTextureBrush()
- Gdip_TextToGraphics()

## 245 NEW FUNCTIONS:

- Unknown source [probably mmikeww]:
  - Gdip_BitmapFromBase64()
  - GetIconDimensions()     

- by Tariq Porter [tic]:
  - Gdip_FillRoundedRectangle2()
  - Gdip_DrawRoundedRectangle2()

- by DevX and Rabiator:
  - Gdip_DrawRoundedLine()

- by SBC:
  - Gdip_GetImageFramesCount()

- by iPhilip:
  - Gdip_SetPenDashStyle()

- 9 by RazorHalo:
  - Gdip_RotatePathAtCenter()
  - Gdip_ResetMatrix()
  - Gdip_RotateMatrix()
  - Gdip_GetPathWorldBounds()
  - Gdip_ScaleMatrix()
  - Gdip_TranslateMatrix()
  - Gdip_TransformPath()
  - Gdip_SetMatrixElements()
  - Gdip_IsVisiblePathPoint()

- 14 by "Learning one":
  - Gdip_AddPathBeziers()
  - Gdip_AddPathBezier()
  - Gdip_AddPathLines()
  - Gdip_AddPathLine()
  - Gdip_AddPathArc()
  - Gdip_AddPathPie()
  - Gdip_SetPathFillMode()
  - Gdip_StartPathFigure()
  - Gdip_ClosePathFigure()
  - Gdip_DrawPath()
  - Gdip_WidenPath()
  - Gdip_ClonePath()
  - Gdip_CombineRegionRegion()
  - Gdip_CreateRegionPath()

- 23 by "Just Me":
  - Gdip_PathGradientCreateFromPath()
  - Gdip_PathGradientSetCenterPoint()
  - Gdip_PathGradientSetCenterColor()
  - Gdip_PathGradientSetSurroundColors()
  - Gdip_PathGradientSetSigmaBlend()
  - Gdip_PathGradientSetLinearBlend()
  - Gdip_PathGradientSetFocusScales()
  - Gdip_AddPathGradient()
  - Gdip_LoadImageFromFile()
  - Gdip_GetPropertyCount()
  - Gdip_GetPropertyIdList()
  - Gdip_GetPropertyItem()
  - Gdip_GetAllPropertyItems()
  - Gdip_GetPropertyTagName()
  - Gdip_GetPropertyTagType()
  - Gdip_GetPropertyItemValue()
  - Multiple Display Monitors Functions by "Just me":
    - GetMonitorCount()
    - GetMonitorInfo()
    - GetPrimaryMonitor()
    - MDMF_FromHWND()
    - MDMF_FromPoint()
    - MDMF_FromRect()
    - MDMF_GetInfo()

- 183 by Marius Șucan [robodesign.ro]:
  - Gdip_DrawStringAlongPolygon()
  - Gdip_InvertMatrix()
  - Gdip_IsMatrixEqual()
  - Gdip_IsMatrixIdentity()
  - Gdip_IsMatrixInvertible()
  - Gdip_MultiplyMatrix()
  - Gdip_GetPenDashStyle()
  - Gdip_SetPenEndCap()
  - Gdip_GetPenEndCap()
  - Gdip_SetPenAlignment()
  - Gdip_GetPenAlignment()
  - Gdip_GetBrushType()
  - Gdip_GetSmoothingMode()
  - Gdip_DrawDrivenString()
  - Gdip_DrawOrientedString()
  - Gdip_CombineRegionPath()
  - Gdip_AddPathStringSimplified()
  - Gdip_CloneFont()
  - Gdip_GetFontFamily()
  - Gdip_CloneFontFamily()
  - Gdip_IsFontStyleAvailable()
  - Gdip_StringFormatGetGeneric()
  - Gdip_GetStringFormatAlign()
  - Gdip_GetStringFormatLineAlign()
  - Gdip_GetStringFormatDigitSubstitution()
  - Gdip_GetStringFormatHotkeyPrefix()
  - Gdip_GetStringFormatTrimming()
  - Gdip_SetStringFormatLineAlign()
  - Gdip_SetStringFormatDigitSubstitution()
  - Gdip_SetStringFormatFlags()
  - Gdip_SetStringFormatHotkeyPrefix()
  - Gdip_SetStringFormatTrimming()
  - Gdip_AddPathString()
  - Gdip_FontFamilyCreateGeneric()
  - Gdip_GetFontHeight()
  - Gdip_GetFontHeightGivenDPI()
  - Gdip_GetFontSize()
  - Gdip_GetFontStyle()
  - Gdip_GetFontUnit()
  - Gdip_GetFontFamilyCellScents()
  - Gdip_GetFontFamilyEmHeight()
  - Gdip_GetFontFamilyLineSpacing()
  - Gdip_GetFontFamilyName()
  - Gdip_GetPathGradientSurroundColors()
  - Gdip_GetPathPoints()
  - Gdip_CloneMatrix()
  - Gdip_GetPenCompoundArray()
  - Gdip_GetPenDashArray()
  - Gdip_RotateBitmapAtCenter()
  - Gdip_RotateLinearGrBrushAtCenter()
  - Gdip_SetLinearGrBrushTransform()
  - Gdip_RotatePathGradientAtCenter()
  - Gdip_PathGradientSetTransform()
  - Gdip_RotateRegionAtCenter()
  - Gdip_TransformRegion()
  - Gdip_SetTextureTransform()
  - Gdip_SetPenTransform()
  - Gdip_GetLinearGrBrushTransform()
  - Gdip_PathGradientGetTransform()
  - Gdip_GetPenTransform()
  - Gdip_GetTextureTransform()
  - Gdip_CreatePathGradient()
  - Gdip_FillClosedCurve2()
  - Gdip_SetPenCompoundArray()
  - Gdip_SetPenDashArray()
  - Gdip_SetPenDashOffset()
  - Gdip_SetPenLineJoin()
  - Gdip_SetPenMiterLimit()
  - Gdip_SetPenUnit()
  - Gdip_GetPenDashCount()
  - Gdip_GetPenDashOffset()
  - Gdip_GetPenLineJoin()
  - Gdip_GetPenMiterLimit()
  - Gdip_GetPenUnit()
  - Gdip_GetPenCompoundCount()
  - Gdip_DrawClosedCurve2()
  - Gdip_AddPathClosedCurve()
  - Gdip_AddPathClosedCurve2()
  - Gdip_AddPathCurve()
  - Gdip_AddPathCurve2()
  - Gdip_GetLinearGrBrushWrapMode()
  - Gdip_SetLinearGrBrushLinearBlend()
  - Gdip_SetLinearGrBrushSigmaBlend()
  - Gdip_SetLinearGrBrushWrapMode()
  - Gdip_GetLinearGrBrushBlendCount()
  - Gdip_PathGradientGetCenterColor()
  - Gdip_PathGradientGetCenterPoint()
  - Gdip_PathGradientGetFocusScales()
  - Gdip_PathGradientGetSurroundColorCount()
  - Gdip_PathGradientTranslateTransform()
  - Gdip_ResetPenTransform()
  - Gdip_RotatePenTransform()
  - Gdip_ScalePenTransform()
  - Gdip_TranslatePenTransform()
  - Gdip_GetPenBrushFill()
  - Gdip_GetPenFillType()
  - Gdip_GetPenStartCap()
  - Gdip_SetPenLineCaps()
  - Gdip_SetPenStartCap()
  - Gdip_CreateCachedBitmap()
  - Gdip_DrawCachedBitmap()
  - Gdip_DeleteCachedBitmap()
  - Gdip_GetTextureImage()
  - Gdip_IsOutlineVisiblePathPoint()
  - Gdip_IsVisibleRegionRectEntirely()
  - Gdip_GetLinearGrBrushGammaCorrection()
  - Gdip_SetLinearGrBrushGammaCorrection()
  - Gdip_GetLinearGrBrushRect()
  - Gdip_ResetLinearGrBrushTransform()
  - Gdip_ScaleLinearGrBrushTransform()
  - Gdip_RotateLinearGrBrushTransform()
  - Gdip_TranslateLinearGrBrushTransform()
  - Gdip_IsClipEmpty()
  - Gdip_IsVisibleClipEmpty()
  - Gdip_IsVisibleGraphPoint()
  - Gdip_IsVisibleGraphRectEntirely()
  - Gdip_IsVisibleGraphRect()
  - Gdip_SetClipFromGraphics()
  - Gdip_GetClipBounds()
  - Gdip_GetVisibleClipBounds()
  - Gdip_GetTextContrast()
  - Gdip_PathGradientGetGammaCorrection()
  - Gdip_PathGradientGetPointCount()
  - Gdip_PathGradientGetRect()
  - Gdip_PathGradientSetGammaCorrection()
  - Gdip_PathGradientSetWrapMode()
  - Gdip_PathGradientGetWrapMode()
  - Gdip_PathGradientResetTransform()
  - Gdip_PathGradientRotateTransform()
  - Gdip_PathGradientScaleTransform()
  - Gdip_GetPathFillMode()
  - Gdip_GetPathLastPoint()
  - Gdip_GetPathPointsCount()
  - Gdip_ResetPath()
  - Gdip_ReversePath()
  - Gdip_GetHatchBackgroundColor()
  - Gdip_GetHatchForegroundColor()
  - Gdip_GetHatchStyle()
  - *Gdip_GetHistogram()
  - Gdip_CreateRegionRect()
  - Gdip_GetWorldTransform()
  - Gdip_CloneRegion()
  - Gdip_SetTextureWrapMode()
  - Gdip_GetTextureWrapMode()
  - Gdip_ScaleTextureTransform()
  - Gdip_RotateTextureTransform()
  - Gdip_ResetTextureTransform()
  - Gdip_ResetTextureTransform()
  - Gdip_TranslateRegion()
  - Gdip_TranslateClip()
  - Gdip_IsEmptyRegion()
  - Gdip_IsEqualRegion()
  - Gdip_IsInfiniteRegion()
  - Gdip_IsVisibleRegionPoint()
  - Gdip_IsVisibleRegionRect()
  - Gdip_SetEmptyRegion()
  - Gdip_SetInfiniteRegion()
  - Gdip_GetRegionBounds()
  - Gdip_GraphicsFlush()
  - Gdip_GetImageBounds()
  - Gdip_GetImageDimension()
  - Gdip_CloneBitmap()
  - Gdip_SetCompositingQuality()
  - Gdip_SetPageScale()
  - Gdip_SetPageUnit()
  - Gdip_SetPixelOffsetMode()
  - Gdip_SetRenderingOrigin()
  - Gdip_SetTextContrast()
  - Gdip_GetCompositingMode()
  - Gdip_GetCompositingQuality()
  - Gdip_GetInterpolationMode()
  - Gdip_GetPageScale()
  - Gdip_GetPageUnit()
  - Gdip_GetPixelOffsetMode()
  - Gdip_GetRenderingOrigin()
  - Gdip_GetTextRenderingHint()
  - Gdip_CreateDIBitmap()
  - Gdip_GetDIBits()
  - Gdip_DrawImageFX()
  - Gdip_BitmapApplyEffect()
  - Gdip_CreateEffect()
  - Gdip_DisposeEffect()
  - GenerateColorMatrix()

(*) mainly written by swagfag, but at my request and modified it further

- 12 by nnnik [extracted from his GDI+ class]:
  - Gdip_DrawBeziers()
  - Gdip_SetLinearGrBrushColors()
  - Gdip_GetLinearGrBrushColors()
  - Gdip_SetSolidFillColor()
  - Gdip_GetSolidFillColor()
  - Gdip_ClonePen()
  - Gdip_SetPenWidth()
  - Gdip_GetPenWidth()
  - Gdip_SetPenColor()
  - Gdip_GetPenColor()
  - Gdip_SetPenBrushFill()
  - Gdip_CreateFontFromDC()

## NOTES:
  - GetProperty() functions yield incorrect results for some meta-data/properties.
  - Gdip_PixelateBitmap() seems to not work for me [in any GDI+ library edition].
  - the newly added examples are not AHK v2 compatible
  - all other tutorials / examples throw an error on script exit on AHK v2 a104; the same applies to @mmikeww's edition
  - awaiting pull requests for bug fixes

## Last updated on: jeudi, 12 septembre 2019, v1.69
